# Module 01 Lab — Completion Record

**Status:** Completed  
**Completion date:** 11 July 2026  
**Environment:** Authorized local Kali Linux lab  
**Target:** Localhost (`127.0.0.1`) only

## Objective

Practise basic Linux navigation, start and verify a local HTTP service, perform
safe service enumeration, capture evidence, and document a mistake and its
correction.

## Authorization and safety

- The target was the tester's own local system.
- Testing was restricted to `127.0.0.1`.
- No public or third-party systems were tested.
- No destructive or denial-of-service actions were performed.

## Commands and actions

```bash
pwd
python3 -m http.server 8000 --bind 127.0.0.1
ss -ltnp | grep ':8000'
nmap -sV -Pn -p 8000 127.0.0.1
curl -I http://127.0.0.1:8000
```

The lab evidence was stored in a dedicated evidence directory with timestamps
and checksums.

## Important output

- The local service listened on `127.0.0.1:8000`.
- Nmap reported `8000/tcp open http`.
- Service detection identified Python `SimpleHTTPServer 0.6`.
- The HTTP request returned `HTTP/1.0 200 OK`.

## Evidence captured

- Start time
- Listening-service output
- Local connectivity test
- Nmap service scan
- HTTP response headers
- SHA-256 evidence manifest
- Screenshots of the important terminal results

Screenshots and raw evidence remain in the private study workspace. They are not
committed because a public repository should contain only sanitized material.

## Mistake

A second HTTP server was started while the original server was already
listening on port 8000. Python returned:

```text
OSError: [Errno 98] Address already in use
```

## Correction

The listening port was checked with `ss`. This confirmed that the original
Python process was already active, so a second server was unnecessary. Nmap and
curl were then run while the original service remained active.

## Final result

The lab objective was achieved:

- [x] Verified the working directory.
- [x] Started a service bound only to localhost.
- [x] Confirmed the listening TCP port.
- [x] Identified the service with Nmap.
- [x] Confirmed an HTTP 200 response.
- [x] Recorded the error and correction.
- [x] Saved evidence for later reporting.

## What I learned

I learned basic Linux commands and how to:

- confirm the current directory;
- start a local Python HTTP server;
- identify which process is using a port;
- distinguish a closed port from an open listening service;
- verify a service with both Nmap and curl;
- treat mistakes as useful evidence instead of hiding them; and
- preserve organized evidence for a penetration-test report.

## Module 01 review tasks

- [x] Write the Module 01 mini-report.
- [x] Create a one-page Module 01 recall sheet.
- [x] Answer ten closed-book recall questions.
- [x] Continue Module 02 after the review is complete.

## Next study task

Continue Module 02 — Penetration Testing Scoping and Engagement.
