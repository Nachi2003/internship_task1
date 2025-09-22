# 🛡️ Cyber Security Internship – Task 1<br>

## 📍 Objective<br>
Discover open ports on devices in your **local network** to understand network exposure and basic reconnaissance techniques.<br>

## 🧰 Tools Used<br>
- **Nmap** – for TCP SYN port scanning<br>
- **Wireshark** *(optional)* – for packet capture and traffic analysis<br>

## 📝 Steps Performed<br>
1. **Install Nmap** from the [official website](https://nmap.org/download.html).<br>
2. **Find Local IP Range** – Identify the subnet (e.g., `192.168.1.0/24`).<br>
3. **Run TCP SYN Scan**:<br>
   ```bash
   nmap -sS 192.168.1.0/24 -oN scan_results.txt
   ```<br>
   `-sS` : TCP SYN (stealth) scan<br>
   `-oN` : Save output in human-readable format (`scan_results.txt`)<br>
4. **Record Findings** – Note active IP addresses and their **open ports**.<br>
5. **Analyze Traffic with Wireshark** – Capture packets and apply a `tcp.flags.syn==1` filter to observe SYN packets.<br>
6. **Research Common Services** running on the discovered ports.<br>
7. **Identify Security Risks** associated with exposed services.<br>
8. **Organize Results** – Save scan output and screenshots inside the repository.<br>
