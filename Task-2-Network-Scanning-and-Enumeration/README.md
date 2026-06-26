🛠️ Module Execution Breakdown

🗺️ 01. Reconnaissance

Objective: Collect technical footprint intelligence using passive data stores and active sweeps.

Key Logs & Proofs: Domain administrative mappings (apexplanet_whois.md, google_whois.md) and verified DNS lookup records (apexplanet_nslookup.md).

Visual Captures: Screenshot verifications for whois data, active ping sweeps, banner grabbing sessions, and advanced dork searches (01_whois.jpg through 05_shodan_google.jpg).

🔍 02. Port & Service Scanning

Objective: Identify accessible entry points, live transmission protocols, and host operating system signatures.

Key Logs & Proofs: Formal documentation manuals (Port_&_Service_Scanning.docx/.pdf) outlining exact Nmap flag syntax combinations.

Visual Captures: Target host sweeps verifying core open port spaces, targeted TCP sequences, stateless UDP configurations, and active OS kernel stack identification maps (01_Nmap_Basic_Scans.jpg to 05_Nmap_OS_Detection.jpg).

📊 03. Vulnerability Scanning

Objective: Deploy automated network scanners to catalog structural security flaws and software vulnerabilities.

Key Logs & Proofs: Complete 110-page raw automated engine evaluation report (meta_2_report.pdf) paired with a compiled risk brief detailing vulnerabilities by threat level.

Visual Captures: Visual step logs illustrating backend architecture startup routines and real-time dashboard risk tracking metrics (01_openVAS_setup.jpg, 02_ulnerability_Report.jpg).

🖧 04. Packet Analysis with Wireshark

Objective: Intercept and parse data-in-transit payloads to trace explicit protocol exposures and DoS signatures.

Key Logs & Proofs: Full analysis reports (Packet_Analysis_with_Wireshark.docx/.pdf) dissecting network streams.

Visual Captures: Step-by-step traffic logs demonstrating cleartext credential harvesting over unencrypted streams, HTTP/DNS captures, and incoming flood fingerprinting (01_HTTP_Capture.jpg to 05_SYN_flood_attack_with_hping3.jpg).

🧱 05. Firewall Basics

Objective: Formulate, configure, and evaluate local kernel packet filtering rules (iptables) to safely shield vulnerable ports.

Key Logs & Proofs: Hardening design configurations and structural rule logs documented cleanly in Firewall_Basics.docx/.pdf.

Visual Captures: Pre-mitigation baseline visibility scans, applied iptables rule architecture configurations, and post-hardening Nmap verification sweeps confirming full port containment (01_firewall_before.jpg to 03_firewall_scans_after_rules_applied.jpg).