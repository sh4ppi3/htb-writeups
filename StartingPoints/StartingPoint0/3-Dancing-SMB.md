# Recon

**nmap -sV $target
```PORT     STATE SERVICE       VERSION
135/tcp  open  msrpc         Microsoft Windows RPC
139/tcp  open  netbios-ssn   Microsoft Windows netbios-ssn
445/tcp  open  microsoft-ds?
5985/tcp open  http          Microsoft HTTPAPI httpd 2.0 (SSDP/UPnP)
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows``
```

# Foothold


Listing SMB repositories with anon user
smbclient -L //$target -p 445 -N

-L: Listing
-N: Anonymous user


conect to target repository with anonymous login
smbclient //target/$repositorio -p 445 -N


# Flag

get flag.txt
5f61c10dffbc77a704d76016a22f1664