# df-mod2-forensic-copy

This project documents the process of creating a forensic copy of evidence files, calculating SHA256 hash values, and verifying that the copies are identical.

The following PowerShell commands were used to calculate SHA256 hashes:

```powershell
# Calculate hash for original evidence files
Get-FileHash .\evidence\filename.ext -Algorithm SHA256

# Calculate hash for forensic copy files
Get-FileHash .\evidence-copy\filename.ext -Algorithm SHA256

#Save the output of a command to a text file
Out-File .\evidence-hashes\filename.ext-hash.txt

#Copy hash for forensic copy files
Out-File .\evidence-copy-hashes\filename.ext-copy-hash.txt

File Name	Original SHA256 Hash	
content.png	61D800A1E92E7537ECFCAC24930879E8058E97D178619705CD59E6042D89C5BB	
            Forensic Copy SHA256 Hash
            61D800A1E92E7537ECFCAC24930879E8058E97D178619705CD59E6042D89C5BB

File Name	Original SHA256 Hash	
doc1.txt	16BBE88D9A7D7619ED86C9C4C712AFD70A3853FF259DA220E8D083693C827F6D	
            Forensic Copy SHA256 Hash
            16BBE88D9A7D7619ED86C9C4C712AFD70A3853FF259DA220E8D083693C827F6D

File Name	Original SHA256 Hash	
file.zip	52724AADA9AE500CBD9CFE6C6E5F3A9294618AB1099084C824E1EA26761C0291	
            Forensic Copy SHA256 Hash
            52724AADA9AE500CBD9CFE6C6E5F3A9294618AB1099084C824E1EA26761C0291

File Name	Original SHA256 Hash	
Notes.docx	7D4731288492FB3AAD8942DBCBC874439517904EEC7387EEA9B190D59CEE440F	
            Forensic Copy SHA256 Hash
            7D4731288492FB3AAD8942DBCBC874439517904EEC7387EEA9B190D59CEE440F  

 File Name	Original SHA256 Hash	
sheet.xlsx	F23BE0EE5F6B8AE42A15F07FF5D9CAB550C6D40400B571AAEF7A2D9D066291C1	
            Forensic Copy SHA256 Hash
            F23BE0EE5F6B8AE42A15F07FF5D9CAB550C6D40400B571AAEF7A2D9D066291C1
            
All file hashes match. 
      
      