# Network Reconnaissance & Port Scanning Audit

## 1. Objective
To understand authorized network reconnaissance, port scanning, service enumeration and packet-level analysis in a controlled training environment.

## 2. Scope
This document uses **SIMULATED/SAMPLE** results for demonstration. No real third-party system was scanned.

## 3. Tools
- Nmap
- Wireshark
- Linux/Kali training environment

## 4. Methodology
Target identification → Host discovery → Port scanning → Service/version enumeration → Packet analysis → Findings → Recommendations

## 5. Sample Nmap Results

| Port | Protocol | Service | Version | Observation |
|---|---|---|---|---|
| 22 | TCP | SSH | OpenSSH 9.2 | Sample exposed service |
| 80 | TCP | HTTP | Apache 2.4 | Sample web service |
| 443 | TCP | HTTPS | Apache 2.4 | Sample encrypted web service |

## 6. Sample Wireshark Analysis
Sample traffic indicates TCP connection establishment between a test client and training host. Packet details are illustrative only.

## 7. Sample Findings
### F-01 – Exposed SSH Service
**Observation:** Port 22 is shown as open in the sample scan.  
**Potential Impact:** An exposed administrative service can increase attack surface.  
**Recommendation:** Restrict access to authorized networks and maintain current security updates.

### F-02 – Web Services
**Observation:** HTTP/HTTPS are shown as open in the sample scan.  
**Recommendation:** Disable unnecessary services and use secure configurations.

## 8. Recommendations
- Close unnecessary ports.
- Disable unused services.
- Restrict administrative access.
- Keep services patched.
- Monitor network traffic.
- Prefer encrypted protocols.

## 9. Conclusion
The exercise demonstrates the workflow for authorized reconnaissance and packet analysis. All results in this package are simulated and should be replaced with genuine lab evidence for an assessed submission.
