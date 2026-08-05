# Recon
PORT      STATE SERVICE       VERSION
135/tcp   open  msrpc         Microsoft Windows RPC
139/tcp   open  netbios-ssn   Microsoft Windows netbios-ssn
445/tcp   open  microsoft-ds?
3389/tcp  open  ms-wbt-server Microsoft Terminal Services (RDP)
5985/tcp  open  http          Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

# Foothold
Lets try to exploit RDP port
3389/tcp  open  ms-wbt-server Microsoft Terminal Services (RDP)
xfreerdp /v:$target /u:Administrator (i got the login with blank password)