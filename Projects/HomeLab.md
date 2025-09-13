# 🛡️ Cybersecurity Home Lab – Learning Journey

## 📖 Overview
Hey there!  

I just completed my first hands-on cybersecurity home lab, and it was an amazing learning experience. I set up **Kali Linux** as my attacker machine and **Metasploitable2** as the target.  

The goal was to safely practice **penetration testing, network scanning, exploitation, and documentation** in a completely isolated environment.  

---

## 🖥️ Lab Setup

| Component | Details |
|-----------|---------|
| Attacker VM | Kali Linux |
| Target VM | Metasploitable2 |
| Network Type | Host-only (VMnet2) |
| Snapshots | Kali: `clean_kali` <br> Metasploitable2: `clean_metasploitable` |

Snapshots saved me a ton of headache — I could always reset the target to a clean state after testing.  

---

## 🛠️ Tools I Used

- 🐧 Kali Linux – Main attacking system  
- 💀 Metasploitable2 – Vulnerable target for practice  
- 🔍 Nmap – Port scanning and service discovery  
- 🗂️ Enum4linux – SMB enumeration  
- 🌐 Nikto & Gobuster – Web service scanning and directory enumeration  
- ⚡ Metasploit Framework – Exploitation  
- 📡 Wireshark – Network traffic capture and analysis  

---

## 🎯 What I Learned

### 1️⃣ Networking and IPs
I learned how to make sure my attacker and target were **on the same isolated network**, and I tested connectivity using `ping`. It was exciting to see everything communicate without touching my real network.

### 2️⃣ Scanning & Enumeration
I ran **full port scans** with Nmap and explored all the open ports on the target. Using Enum4linux, Nikto, and Gobuster, I got a feel for how attackers gather information before exploiting a system.

### 3️⃣ Exploitation
This part was thrilling!  
- Found the **vsftpd 2.3.4 backdoor** using Searchsploit.  
- Used Metasploit to safely get a shell on the target VM.  
- Ran commands like `whoami`, `id`, and `ls` to explore the system.  

This helped me understand how scanning, enumeration, and exploitation fit together.

### 4️⃣ Network Analysis
Captured traffic with Wireshark to observe:  
- ✅ TCP handshakes  
- ⚡ Reverse shell connections  
- 🌐 HTTP requests/responses  

It was fascinating to see the invisible flow of data during the exploit.

### 5️⃣ Documentation & Lab Hygiene
Documented everything:  
- Commands I ran  
- Scan outputs  
- Exploit results  
- Screenshots  

Snapshots allowed me to **revert the target VM** to a clean state after each experiment, which is super helpful for repeated practice.

---

## 💡 Best Practices Learned

- Always use **isolated networks** for safety  
- Take **snapshots** before and after experiments  
- Document everything carefully — it helps later  
- Practice ethical hacking only in controlled lab environments  

---

## 🚀 Next Steps

- Add a **Windows VM** to practice Active Directory attacks  
- Add an **Ubuntu server** for ELK/Wazuh logging practice  
- Deploy **pfSense** as a lab router/firewall  
- Explore other vulnerable services and capture traffic for analysis  

---

## ✨ Summary

This lab was my first real dive into **ethical hacking and penetration testing**. I learned:  
- The full workflow: **Scan → Enumerate → Exploit → Post-Exploit → Document**  
- Safe lab practices and VM snapshots  
- Network traffic analysis  
- Proper documentation  

Excited to continue building more labs and expanding my cybersecurity skills!
