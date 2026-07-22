# **Theory Question**

1.  In cybersecurity, isolated environments—like Pwnbox or the vulnerable target machines—are often VMs. What does VM stand for?
**R: Virtual Machine**

2. What tool do we use to interact with the operating system in order to issue commands via the command line, such as the one to start our VPN connection? It's also known as a console or shell.
**R: Terminal**

3. What service do we use to form our VPN connection into HTB labs?
**R: OpenVPN**

4. What tool do we use to test our connection to the target with an ICMP echo request?
**R: Ping**

5. What is the name of the most common tool for finding open ports on a target?
**R: Nmap**


# **Reconnaissance**

6. What service do we identify on port 23/tcp during our scans?
**R: `nmap -sV $TARGET`**


# **Exploit**

7. What username is able to log into the target over telnet with a blank password?
**R: `root` (Always test default credentials if you can)**

8. Submit the flag located in root's home directory.
**R: After telnet connection. I just had to `ls`  / directory.**