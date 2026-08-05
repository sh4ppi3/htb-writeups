# Recon
nmap to discover port 80 open


# Enumeration
ffuf to discover admin.php subdirectory
`ffuf -w wordlist -u  http://$target/ -x php`


# Foothold
testing with default credentials on admin.php
got it with admin/admin
