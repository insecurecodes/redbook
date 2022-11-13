---
description: >-
  The File Transfer Protocol is a standard communication protocol used for the
  transfer of computer files from a server to a client on a computer network.
  FTP is built on a client–server model architect
---

# FTP

{% hint style="info" %}
Default port: **21**
{% endhint %}

### Enum

```bash
nmap $IP -p 21 -sV -O
```

### Bruteforce with Hydra

{% code overflow="wrap" %}
```shell
hydra -L /usr/share/metasploit-framework/data/wordlists/unix_users.txt -P /usr/share/metasploit-framework/data/wordlists/unix_passwords.txt $IP ftp
```
{% endcode %}

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

### Bruteforce with Nmap

{% code overflow="wrap" %}
```shell
nmap $IP --script ftp-brute --script-args userdb=/path/to/users -p 21
```
{% endcode %}

## Anonymous Login

```bash
nmap $IP --script ftp-anon
```

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
