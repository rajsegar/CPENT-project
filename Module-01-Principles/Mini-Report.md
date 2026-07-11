# Module 01 Mini Report — Scope, Authorization, and Evidence

**Status:** Completed  
**Tester:** RedteamAI  
**Module:** CPENT Module 01 — Principles and Objectives of Penetration Testing  
**Assessment type:** Authorized local lab assessment  
**Completion date:** 11 July 2026  
**Environment:** Kali Linux local lab  
**Target:** `127.0.0.1:8000` only

## 1. Executive Summary

This mini-assessment was completed as part of CPENT Module 01 practical learning.

The purpose of the assessment was to practise the professional penetration testing process before moving into deeper technical testing. The lab focused on authorization, scope, safe target selection, basic service verification, evidence collection, and reporting.

Testing was performed only against the tester's own local system using a Python HTTP service bound to localhost. No public websites, third-party systems, production services, or unrelated network devices were tested.

## 2. Scope

### In Scope

```text
Target: 127.0.0.1
Port: 8000
Service: Local Python HTTP server
Environment: Local Kali Linux lab
Purpose: Safe service verification and evidence practice
```

### Out of Scope

```text
Public websites
Real company systems
Home router
Other devices on the network
Other local services not required for the lab
Denial of Service testing
Destructive testing
Social engineering
Credential attacks against real accounts
```

## 3. Authorization and Safety

The assessment was authorized because the target was a self-owned local lab service running on the tester's own system.

The HTTP service was restricted to `127.0.0.1`, which means it was intended to be reachable only from the local machine.

Safety rules followed during the lab:

- Only localhost was tested.
- No public or third-party systems were tested.
- No destructive actions were performed.
- No denial-of-service activity was performed.
- Evidence was sanitized before being committed to the public repository.

## 4. Rules of Engagement

```text
Allowed:
- Basic Linux navigation
- Starting a local HTTP service
- Checking listening ports
- Safe service enumeration
- HTTP header verification
- Screenshot and evidence collection

Not allowed:
- Testing public websites
- Testing third-party systems
- Testing unrelated network devices
- Denial of Service
- Destructive payloads
- Persistence
- Malware
```

## 5. Methodology

This assessment followed the Module 01 penetration testing process.

### Pre-Attack Phase

The tester confirmed authorization, defined the local target, selected safe commands, and prepared evidence collection.

### Attack Phase

No exploitation was performed. The lab only verified that the local service was running and identifiable.

### Post-Attack Phase

The tester reviewed evidence, documented the result, recorded a mistake and correction, and preserved sanitized notes for the study repository.

## 6. Evidence Summary

Commands used:

```bash
pwd
python3 -m http.server 8000 --bind 127.0.0.1
ss -ltnp | grep ':8000'
nmap -sV -Pn -p 8000 127.0.0.1
curl -I http://127.0.0.1:8000
```

Important results:

```text
The local service listened on 127.0.0.1:8000.
Nmap reported 8000/tcp open http.
Service detection identified Python SimpleHTTPServer 0.6.
The HTTP request returned HTTP/1.0 200 OK.
```

Evidence captured:

- Start time
- Listening-service output
- Local connectivity test
- Nmap service scan
- HTTP response headers
- SHA-256 evidence manifest
- Screenshots of important terminal results

Raw screenshots and full evidence remain in the private study workspace. Only sanitized information is committed to the public repository.

## 7. Finding

### Finding Title

Local HTTP Service Exposed for Training

### Affected Target

```text
127.0.0.1:8000
```

### Observation

A Python HTTP service was running locally on port 8000 and responding to HTTP requests.

### Evidence

```text
ss confirmed a listening service on port 8000.
Nmap identified 8000/tcp as open and running HTTP.
curl confirmed an HTTP/1.0 200 OK response.
```

### Impact

In this lab, the impact was controlled because the service was bound to localhost and used only for training. If a similar test service were exposed to an untrusted network, it could unintentionally reveal files from the directory where the server was started.

### Severity

Informational

### Remediation

Keep training services bound to localhost unless network access is intentionally required. Stop temporary services when the lab is complete. Do not run temporary HTTP servers from directories containing sensitive files.

## 8. Mistake and Correction

### Mistake

A second HTTP server was started while the first server was already listening on port 8000. Python returned:

```text
OSError: [Errno 98] Address already in use
```

### Correction

The listening port was checked with `ss`, which confirmed that the original Python process was already active. Nmap and curl were then run against the existing service.

## 9. Cleanup

```text
No public systems were tested.
No destructive changes were made.
The local service can be stopped after the lab.
Evidence was saved and sanitized for study documentation.
```

## 10. What I Learned

This lab showed that a professional penetration test starts with authorization, scope, and rules before technical testing. I also learned how to verify a local service, collect evidence, document mistakes, and explain a result in a report format.

## 11. Final Status

```text
Module 01 mini-report: Completed
Module 01 practical lab: Completed
Module 01 evidence: Recorded and sanitized
Ready for Module 02: Yes
```
