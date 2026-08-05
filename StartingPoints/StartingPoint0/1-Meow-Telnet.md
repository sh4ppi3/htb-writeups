# Recon
```
Command: nmap -sV -p- --min-rate 5000 $target

Starting Nmap 7.98 ( https://nmap.org ) at 2026-08-01 09:16 -0300
Nmap scan report for 10.129.42.23
Host is up (0.16s latency).
Not shown: 65534 closed tcp ports (reset)
PORT   STATE SERVICE VERSION
23/tcp open  telnet  Linux telnetd
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel
```

# Foothold
 Testing for exposed telnet service
`Command: telnet $target

![Pasted image 20260801092552](../../Images/Pasted%20image%2020260801092552.png)

Testing with default credentials: `root` And we got the login.

# Flag

![Pasted image 20260801092645.png](../../Images/Pasted%20image%2020260801092645.png)