# Nmap Practice Scan - scanme.nmap.org

## 1. Objective
Practice network scanning and service version detection
using the Nmap project's designated testing server.

## 2. Target
- Domain: scanme.nmap.org
- Resolved IPv4: 45.33.32.156
- Tool: Nmap 7.991
- Operating System: Kali Linux 2026.3

## 3. Command Executed
nmap -sV -oA Zenmap/scans/scanme-basic scanme.nmap.org

## 4. Scan Results

### Open Ports
| Port | Service | Version |
|---|---|---|
| 22/tcp | tcpwrapped | Not identified |
| 80/tcp | HTTP | Apache 2.4.7 |
| 9929/tcp | Nping Echo | Not specified |

### Filtered Ports
23, 24, 25, 135, 139, 445

### Closed Ports
991 TCP ports reported closed.

## 5. Analysis
The target responded to Nmap scanning.

Three open TCP ports were identified.
Six listed ports were filtered.
The remaining 991 TCP ports were reported closed.

The HTTP service was identified as Apache 2.4.7
on Ubuntu according to Nmap service detection.

Filtered ports did not provide sufficient information
to determine whether services were running.

## 6. Limitations
- Service detection does not prove vulnerabilities.
- No exploitation was attempted.
- No vulnerability assessment was performed.
- Results reflect the scan time only.

## 7. Evidence
- ../scans/scanme-basic.nmap
- ../scans/scanme-basic.xml
- ../scans/scanme-basic.gnmap

## 8. Conclusion
The exercise successfully demonstrated TCP port discovery
and service version detection using Nmap.
