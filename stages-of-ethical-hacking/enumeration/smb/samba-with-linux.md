# Samba with Linux

## Enumeration

With nmap `-sV` we can do an educated guess if the server is using <mark style="background-color:blue;">windows</mark> or <mark style="background-color:purple;">linux</mark>

```shell
- TCP
nmap $IP -sV -p 139,445

- UDP
nmap $IP -sU --top-port 25 --open

- Via scripts
nmap $IP -p 445 --script smb-os-discovery
```

<figure><img src="../../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

## Metasploit way



```bash
```
