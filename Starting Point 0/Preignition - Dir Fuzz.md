nmap to discover port 80 open

ffuf to discover admin.php subdirectory
ffuf -w wordlist -u  http://$target/ -x php

testing with default credentials on admin.php
got it with admin/admin
