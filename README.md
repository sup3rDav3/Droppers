# Dropper
Coursework from Sektor7's final project  
https://institute.sektor7.net/view/courses/red-team-operator-malware-development-essentials

The final dropper does the following:
+ Shellcode = message box (via notepad.exe)
+ Extracts shellcode from .rsrc
+ Decrypts shellcode (XOR)
+ Injects shellcode into notepad.exe
+ Make it a GUI instead of console app (eliminate pop-up)

1. Encrypt payload with:  
python.exe xorencrypt.py msgbox64.bin (this creates favicon.ico = XOR encrypted payload)
2. Run compile.bat
3. Run implant.exe

TODO:
Add reverse shell payload
Bypass Defender
