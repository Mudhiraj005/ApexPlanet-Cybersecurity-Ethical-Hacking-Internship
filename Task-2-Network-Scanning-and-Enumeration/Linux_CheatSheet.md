# Cybersecurity Internship: Task 2 Linux Command Cheat Sheet

This cheat sheet indexes all network reconnaissance, port scanning, vulnerability validation, packet manipulation, and firewall rules used throughout Tasks 2.1 to 2.5.

---

## Task 2.1: Passive & Active Reconnaissance

### 1. `whois`
* **Use Case:** Passive domain information gathering.
* **Syntax Example:** `whois apexplanet.in` or `whois google.com`
* **Simple Description:** Queries the global registrar database to gather domain ownership records, creation/expiry dates, hostnames, and technical administrative contacts.

### 2. `nslookup`
* **Use Case:** DNS query verification.
* **Syntax Example:** `nslookup apexplanet.in`
* **Simple Description:** Maps a user-friendly domain name to its corresponding public IPv4 or IPv6 addresses by directly querying Domain Name System (DNS) servers.

### 3. `nmap -sn`
* **Use Case:** Ping Sweep (Active Reconnaissance).
* **Syntax Example:** `nmap -sn 192.168.56.0/24`
* **Simple Description:** Scans an entire block of network IP addresses to see which systems are alive and responding, without running intensive port-level checks.

---

## Task 2.2: Port & Service Scanning

### 4. `nmap -sS`
* **Use Case:** Stealthy TCP Port Mapping.
* **Syntax Example:** `nmap -sS 192.168.56.101`
* **Simple Description:** Performs a "half-open" TCP SYN scan. It sends a connection request but tears it down before it completes, allowing you to discover open ports quickly while minimizing network log entries.

### 5. `nmap -sU`
* **Use Case:** UDP Port Mapping.
* **Syntax Example:** `nmap -sU 192.168.56.101`
* **Simple Description:** Scans for open UDP ports to reveal hidden attack surfaces like DNS, DHCP, or SNMP services that don't use standard TCP handshakes.

### 6. `nmap -sV`
* **Use Case:** Service Version Detection / Banner Grabbing.
* **Syntax Example:** `nmap -sV 192.168.56.101`
* **Simple Description:** Interrogates open network ports to capture software banners, identifying the exact application names and software version numbers running on the host.

### 7. `nmap -O`
* **Use Case:** Operating System Fingerprinting.
* **Syntax Example:** `nmap -O 192.168.56.101`
* **Simple Description:** Analyzes minor variations in how the target's network card responds to probe packets to accurately guess the remote operating system type and kernel version.

---

## Task 2.3: Vulnerability Assessment (OpenVAS Framework)

### 8. `gvm-start`
* **Use Case:** Launching OpenVAS services.
* **Syntax Example:** `sudo gvm-start`
* **Simple Description:** Starts up the local Greenbone Vulnerability Manager backend daemons and initializes the web user interface on the Kali Linux platform.

### 9. `gvm-check-setup`
* **Use Case:** Installation diagnostics.
* **Syntax Example:** `sudo gvm-check-setup`
* **Simple Description:** Runs a diagnostic script that checks your OpenVAS components, directories, and permissions to make sure the scanner is fully operational.

### 10. `gvm-feed-update`
* **Use Case:** Updating signature databases.
* **Syntax Example:** `sudo gvm-feed-update`
* **Simple Description:** Synchronizes your engine with the latest global database of Network Vulnerability Tests (NVTs) so the scanner can detect newly discovered security flaws.

---

## Task 2.4: Packet Analysis & Attack Simulation

### 11. `wireshark`
* **Use Case:** Packet Sniffing & Traffic Analysis.
* **Syntax Example:** `sudo wireshark`
* **Simple Description:** Launches a graphical packet analyzer tool that intercepts and decodes live network traffic to inspect raw payloads (such as unencrypted FTP usernames and passwords).

### 12. `hping3 --flood -S`
* **Use Case:** SYN Flood DoS Attack Simulation.
* **Syntax Example:** `sudo hping3 --flood -S 192.168.56.101`
* **Simple Description:** Generates and fires TCP SYN connection packets at a target server as fast as possible to simulate a Denial of Service (DoS) attack and test network baseline defenses.

---

## Task 2.5: Defensive Firewall Architecture

### 13. `iptables -L`
* **Use Case:** Inspecting active firewall rules.
* **Syntax Example:** `sudo iptables -L -v -n`
* **Simple Description:** Lists all current packet-filtering configuration lines currently running inside the Linux kernel network stack.

### 14. `iptables -A INPUT ... -j ACCEPT`
* **Use Case:** Permitting legitimate service traffic.
* **Syntax Example:** `sudo iptables -A INPUT -p tcp --dport 21 -j ACCEPT`
* **Simple Description:** Appends a configuration rule to explicitly allow incoming connections targeting a specific port (e.g., permitting FTP traffic on Port 21).

### 15. `iptables -A INPUT ... -j DROP`
* **Use Case:** Silently blocking unauthorized services.
* **Syntax Example:** `sudo iptables -A INPUT -p tcp --dport 22 -j DROP`
* **Simple Description:** Discards incoming packets for a specified port (e.g., SSH on Port 22) without sending an error notification back, leaving the port appearing completely dead to external scanners.

### 16. `iptables -A INPUT ... -j REJECT`
* **Use Case:** Actively denying prohibited traffic.
* **Syntax Example:** `sudo iptables -A INPUT -p tcp --dport 23 -j REJECT`
* **Simple Description:** Blocks connection attempts (e.g., Telnet on Port 23) while explicitly sending a "Destination Unreachable" response back to notify the sender that access is denied.

### 17. `iptables -F`
* **Use Case:** Resetting firewall configurations.
* **Syntax Example:** `sudo iptables -F`
* **Simple Description:** Flushes (erases) all custom user-defined rules across all firewall chains, resetting the system back to its baseline default policy behaviors.