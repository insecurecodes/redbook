---
description: >-
  The Modern Port Scanner. Find ports quickly (3 seconds at its fastest). Run
  scripts through our scripting engine (Python, Lua, Shell supported).
---

# RustScan

## ✨ Features

* Scans all 65k ports in **3 seconds**.
* Full scripting engine support. Automatically pipe results into Nmap, or use our scripts (or write your own) to do whatever you want.
* Adaptive learning. RustScan improves the more you use it. No bloated machine learning here, just basic maths.
* The usuals you would expect. IPv6, CIDR, file input and more.
* Automatically pipes ports into Nmap.

{% embed url="https://github.com/RustScan/RustScan" %}

## Installation

```bash
brew install rustscan
```

## Default Scan

```bash
# Simple Scan
rustscan -a $DOMAIN

# Increase speed with ulimit (can cause rejection of host)
rustscan -a $DOMAIN --ulimit 5000

# Specify port
rustscan -a $DOMAIN -p 443

# Multiple ports
rustscan -a $DOMAIN -p 443,80,3306,9000,8080

# Range of ports
rustscan -a $DOMAIN --range 1-1000

# Scan network
rustscan -a 192.168.0.0/24
```

## Advanced Scan

<mark style="color:red;">`TO BE DONE`</mark>

## Scripts

<mark style="color:red;">`TO BE DONE`</mark>
