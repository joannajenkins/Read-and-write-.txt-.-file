# Read-and-write-.txt-.-file
Read and write .txt . file
 Save file txt
FileOutputStream fos = openFileOutput("khoapham.txt", Context.MODE_PRIVATE); 
fos.write(noidung.getBytes());
fos.close()

- Read file txt
FileInputStream fis = openFileInput("khoapham.txt"); 
BufferedReader br = new BufferedReader(new InputStreamReader(new DataInputStream(fis))); 
String line = ""; 
while( (line = br.readLine()) != null ){ 
txtvNoiDung.append(line); 
txtvNoiDung.append("\n"); 
}
