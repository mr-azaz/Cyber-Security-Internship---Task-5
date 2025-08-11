# Cyber-Security-Internship---Task-5
# 🛠 Task 5 – Capture and Analyze Network Traffic Using Wireshark

## 📌 Objective
Capture live network packets and identify at least 3 protocols using Wireshark.

## 📂 Files Included
- `network_capture_task5.pcap` – Raw packet capture file.
- `README.md` – This report summarizing actions, tools used, and findings.
- `Wireshark_Report_Task5.docx` – Detailed explained report with step-by-step analysis and observations.

## 📜 Steps Performed
1. Installed Wireshark on Kali Linux.
2. Started capture on the active network interface.
3. Visited the website **[elevateapp.com](https://elevateapp.com)** to generate HTTP/HTTPS and DNS traffic.
4. Used `ping` to test connectivity to a remote server.
5. Stopped capture after ~1 minute.
6. Filtered captured traffic by protocol (`dns`, `http`, `icmp`).
7. Saved the capture as `network_capture_task5.pcap`.

## 🔍 Protocols Observed
1. **DNS** – Resolved `elevateapp.com` and other domains to IP addresses.  
   - Example: Standard query `A elevateapp.com`.
2. **HTTP/HTTPS** – Web traffic to **elevateapp.com**.
   - HTTPS traffic encrypted, HTTP payload visible in plain text.
3. **ICMP** – Ping requests and replies.  
   - Example: Echo Request from **192.168.220.8** to **104.26.7.47**, and Echo Reply back.

## 📊 Findings
- DNS used UDP to perform domain name resolution.
- HTTP packets showed request/response details, while HTTPS was encrypted.
- ICMP confirmed network connectivity between the local host and the remote IP **104.26.7.47**.
- The majority of traffic observed was TCP-based.

## 🎯 Outcome
Successfully captured live traffic, identified multiple protocols, and analyzed packet details using Wireshark.

---
