---
description: >-
  Nikto is an Open Source (GPL) web server scanner which performs comprehensive
  tests against web servers for multiple items, including over 6700 potentially
  dangerous files/programs, etc ...
---

# Nikto

## Installation and introduction

{% embed url="https://github.com/sullo/nikto" %}

## Default scan

```bash
# HTTP
nikto -h $DOMAIN

# HTTPS
nikto -h $DOMAIN -ssl

# Use domains from file
nikto -h domains.txt
```

#### Output&#x20;

```bash
# Simple
nikto -h $DOMAIN -o output.txt

# CSV format
nikto -h $DOMAIN -o output.csv -Format csv
```

#### Integration with metasploit

```bash
nikto -h $DOMAIN -Format msf+
```

## Advanced scan

<mark style="color:red;">`TO BE DONE`</mark>
