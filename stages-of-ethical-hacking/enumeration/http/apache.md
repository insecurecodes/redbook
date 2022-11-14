---
description: >-
  The Apache HTTP Server Project is an effort to develop and maintain an
  open-source HTTP server for modern operating systems including UNIX and
  Windows.
---

# Apache

## Enum

```bash
nmap $IP -p 80 -sV -O

nmap $IP -p 80 -sV --script banner

whatweb $IP

http $IP

dirb http://$IP 

browsh --startup-url $IP

lynx http://$IP

# Metasploit version
msfconsole
use auxiliary/scanner/http/http_version
set rhosts $IP
run

# Metasploit directiries
msfconsole
use auxiliary/scanner/http/brute_dirs
set rhosts $IP
run

#robots.txt
msfconsole
use auxiliary/scanner/http/robots_txt
set rhosts $IP
run
```
