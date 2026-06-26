# Module 01 — Commands

Module 01 is mostly theory, but these commands support the Pre-Attack phase.

## Basic host discovery

```bash
ping -c 4 <target-ip>
```

Purpose: Check whether the host responds to ICMP.

## Basic Nmap scan

```bash
nmap <target-ip>
```

Purpose: Find common open TCP ports.

## Service detection

```bash
nmap -sV <target-ip>
```

Purpose: Identify services and versions.

## Safer scan when ping is blocked

```bash
nmap -Pn <target-ip>
```

Purpose: Treat the host as alive even if ICMP is blocked.

## Full TCP port scan

```bash
nmap -p- <target-ip>
```

Purpose: Check all 65535 TCP ports.

## Common practical scan

```bash
nmap -sC -sV -Pn -oN nmap-basic.txt <target-ip>
```

Purpose:

- `-sC`: Run default scripts
- `-sV`: Detect service versions
- `-Pn`: Skip host discovery
- `-oN`: Save output to a normal text file

## HTTP header check

```bash
curl -I http://<target>
```

Purpose: View HTTP response headers.

## DNS lookup

```bash
dig <domain>
```

Purpose: Query DNS records.

## WHOIS lookup

```bash
whois <domain>
```

Purpose: Find domain registration information.

## Important reminder

Only run scans against systems where you have permission.
