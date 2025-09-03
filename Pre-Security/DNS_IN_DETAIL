# 🌐 DNS (Domain Name System)

DNS (Domain Name System) is like the **phonebook of the internet**.  
It translates **human-friendly names** (like `tryhackme.com`) into **machine-friendly IP addresses** (like `104.26.10.229`).  

Instead of remembering numbers, we just type names — and DNS handles the rest.

---

## 🏠 Analogy
- Every house has a **unique address** → Every device has an **IP address**.  
- Instead of memorizing house addresses, we just remember **names**.  
- DNS maps **names → addresses** automatically.  

---

## 🏷️ Domain Name Structure
A full domain like `admin.tryhackme.com` can be broken down into parts:

- **TLD (Top-Level Domain)** → The rightmost part of a domain.  
  - Example: `.com`, `.org`, `.gov`, `.edu`  
  - **gTLD (Generic TLD):** `.com`, `.org`, `.edu`, `.gov`, `.online`, `.club`, etc.  
  - **ccTLD (Country Code TLD):** `.in` (India), `.ca` (Canada), `.co.uk` (UK)  

- **Second-Level Domain** → The main name chosen by the owner.  
  - Example: In `tryhackme.com`, **tryhackme** is the second-level domain.  

- **Subdomain** → Comes before the second-level domain.  
  - Example: `admin.tryhackme.com` → Here, **admin** is the subdomain.  
  - You can chain subdomains: `jupiter.servers.tryhackme.com`.  

---

## 📂 Common DNS Record Types
DNS doesn’t just map websites — it stores many types of records:

- **A Record** → Maps a domain to an IPv4 address.  
  - Example: `tryhackme.com → 104.26.10.229`  

- **AAAA Record** → Maps a domain to an IPv6 address.  
  - Example: `tryhackme.com → 2606:4700:20::681a:be5`  

- **CNAME Record** → Points one domain name to another.  
  - Example: `store.tryhackme.com → shops.shopify.com`  

- **MX Record** → Tells which server handles emails for a domain.  
  - Example: `alt1.aspmx.l.google.com` (for Gmail).  

- **TXT Record** → Stores free text data.  
  - Uses:  
    - Verify domain ownership.  
    - Fight spam (email authentication like **SPF, DKIM**).  

---

## 🔄 How a DNS Request Works
When you type `tryhackme.com` in your browser:

1. **Check Local Cache**  
   - Your computer first checks if it already knows the IP.  

2. **Ask Recursive DNS Server**  
   - Usually provided by your ISP (or Google DNS like `8.8.8.8`).  
   - If cached, it replies immediately.  

3. **If Not Cached → Go to Root Servers**  
   - Root servers act as the **backbone of DNS**.  
   - They point you to the right TLD server (`.com`, `.org`, etc.).  

4. **TLD Server → Authoritative Server**  
   - The TLD server tells you which **authoritative server** holds the records.  
   - Example for `tryhackme.com`: `kip.ns.cloudflare.com`.  

5. **Authoritative Server → Final Answer**  
   - This server returns the **actual IP address** of the domain.  

6. **Caching**  
   - The result is cached at each step with a **TTL (Time To Live)** value (in seconds).  
   - Example: If `TTL = 300`, your system won’t ask again for 5 minutes.  

---

## ✅ Key Takeaways
- DNS = **Phonebook of the internet**  
- Converts **domain names → IP addresses**  
- A domain = **TLD + Second-Level Domain + (optional) Subdomain**  
- Many record types exist (**A, AAAA, CNAME, MX, TXT**)  
- DNS resolution involves:  
  **Local Cache → Recursive DNS → Root Server → TLD Server → Authoritative Server**  
