T1059.001 - PowerShell

Evidence:
powershell.exe -enc

T1027 - Obfuscated Files or Information

Evidence:
Base64 Encoded Command

T1562.001 - Impair Defenses

Evidence:
AmsiUtils
amsiInitFailed=True

T1105 - Ingress Tool Transfer

Evidence:
DownloadData()

T1071.001 - Web Protocols

Evidence:
https://45.77.65.211/admin/get.php
