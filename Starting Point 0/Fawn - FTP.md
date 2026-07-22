# **Theory Question**

1. What does the 3-letter acronym FTP stand for?
R: **File Transfer Protocol**

2. Which port does the FTP service listen on usually?
R: **21**

3. FTP sends data in the clear, without any encryption. What acronym is used for a later protocol designed to provide similar functionality to FTP but securely, as an extension of the SSH protocol?
**R: SFTP (SSH File Transfer Protocol, in the other words, its the FTP protocol protected by SSH cryptography)

4. What is the command we can use to send an ICMP echo request to test our connection to the target?
R: **Ping**

# **Reconnaissance**

5. From your scans, what version is FTP running on the target?
R: **To identify exposed processes on ports names you need to run `nmap -sV $TARGET` - It is running `vsftpd 3.0.3**`

6. From your scans, what OS type is running on the target?
R: **We got that from the nmap command also: Unix**

7. What is the command we need to run in order to display the 'ftp' client help menu?
R: **`ftp -?`**



# **Exploit**

8. What is username that is used over FTP when you want to log in without having an account?
R: **anonymous**

9. What is the response code we get for the FTP message 'Login successful'?
R: **230**

10. There are a couple of commands we can use to list the files and directories available on the FTP server. One is dir. What is the other that is a common way to list files on a Linux system.
R: **`ls`**

11. What is the command used to download the file we found on the FTP server?
R: **`Get`** 

12. Flag
R: **Got with `Get` command on flag.**

