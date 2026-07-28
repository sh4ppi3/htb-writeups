nmap -sV $target

PORT     STATE SERVICE       VERSION
135/tcp  open  msrpc         Microsoft Windows RPC
139/tcp  open  netbios-ssn   Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds?
5985/tcp open  http          Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows



Listar portas SMB com usuário anonimo
smbclient -L //$target -p 445 -N

-L: Listar
-N: Anonimo
-U: Usuario


Conectar a repositório aberto
smbclient //$target/$repositorio -p 445 -N

get flag.txt


5f61c10dffbc77a704d76016a22f1664