# network-security-scan
Nmap and Wireshark-based network scanning and analysis
# Network Security Scan Repository

This repository contains network security scan results, including Nmap and Wireshark capture files.

## Capture Files Description

- **ip.addr captured 64-14.pcapng**  
  Wireshark capture file containing network traffic filtered by IP address range 64-14. Includes detailed packet-level data useful for analyzing communications within this IP scope.

- **ip_addr_capture_1.pcapng**  
  Wireshark capture file focusing on specific network traffic patterns, such as handshake events or traffic on certain ports. Useful for deeper inspection of network behavior.

- **scan_result.txt**  
  Nmap scan output with open ports and service details.

## Research on Common Services Running on These Ports

Based on the Nmap scan results and Wireshark captures, typical services running on the discovered open ports may include:

- **Port 22 (SSH):** Secure Shell for remote administration; risk includes brute force attacks if weak passwords are used.
- **Port 80 (HTTP) / 443 (HTTPS):** Web services; risks include outdated web servers vulnerable to exploits.
- **Port 53 (DNS):** Domain Name System service; risks include DNS spoofing or cache poisoning attacks.
- **Port 445 (SMB):** Windows file sharing; high risk if exposed, prone to ransomware and malware exploitation.
- **Other high-numbered ports:** Often used by custom or ephemeral services; risks depend on service configuration and exposure.

## Potential Security Risks from Open Ports

Open ports expose services to the network and may lead to:

- Unauthorized access if services are misconfigured or unpatched.
- Exposure to known vulnerabilities and exploits targeting those services.
- Information leakage through banners or misconfigured protocols.
- Network reconnaissance by attackers to map services and plan attacks.
- Denial of Service (DoS) attacks exploiting open ports or services.

---

## Recommendations

- Regularly update and patch all services.
- Limit exposure of critical ports to trusted networks or VPNs.
- Use strong authentication methods and monitor login attempts.
- Employ firewalls and intrusion detection/prevention systems.
- Conduct regular vulnerability assessments and penetration tests.

---

Feel free to analyze the capture files using Wireshark or similar tools for detailed network traffic inspection.
