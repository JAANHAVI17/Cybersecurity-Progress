# BrightLayer Stores – Cybersecurity Risk Assessment

## 📌 Project Overview

This project presents a basic cybersecurity risk assessment for **BrightLayer Stores**, a simulated small business with 8 employees.

The assessment follows the standard cybersecurity risk analysis flow:

**Asset → Threat → Vulnerability → Risk → Recommendation**

The goal is to identify important business assets, understand potential threats and weaknesses, evaluate their possible impact, and suggest practical security improvements.

---

## 🏢 Scenario

**BrightLayer Stores** is a simulated business with 8 employees. Its technology environment includes:

- Employee email accounts
- Shared computers
- Company website
- Cloud storage containing invoices
- User passwords
- Public Wi-Fi router

---

# 1. FIVE IMPORTANT ASSETS

### 1. Employee Email Accounts

Used for internal and customer communication, password resets, and sharing business information. Compromised accounts could expose sensitive company information.

### 2. Cloud Storage

Contains invoices and other important business documents. Loss or unauthorized access could affect financial records and daily operations.

### 3. Company Website

Provides an online presence for the business. A compromised or unavailable website could affect customer trust and business operations.

### 4. Employee Passwords

Passwords protect email, cloud storage, and other systems. Weak or reused passwords could allow unauthorized access.

### 5. Shared Computers and Public Wi-Fi Router

Shared computers are used for daily business activities, while the router provides network access. A compromise could provide attackers with access to company systems or information.

---

# 2. THREE POTENTIAL THREATS

### 1. Phishing / Credential Theft

**Threat Actor:** Cybercriminal attempting to trick employees into revealing passwords through fake emails or login pages.

### 2. Malware Infection

**Threat Actor/Event:** Malware introduced through malicious attachments, downloads, or compromised websites.

### 3. Unauthorized Network Access

**Threat Actor:** An attacker attempting to exploit an insecure or poorly configured public Wi-Fi router.

---

# 3. THREE VULNERABILITIES

### 1. Weak or Reused Passwords

Employees may use simple or identical passwords across multiple business services.

### 2. Insufficient Security Controls on Shared Computers

Shared computers may lack individual user accounts, automatic screen locking, updated antivirus software, or restrictions on software installation.

### 3. Poorly Secured Wi-Fi Router

The router may have outdated firmware, weak administrator credentials, or insufficient separation between public users and company devices.

---

# 4. ASSOCIATED RISKS

| Threat | Vulnerability | Potential Impact |
|---|---|---|
| Phishing / Credential Theft | Weak or reused passwords | Unauthorized access to email and cloud storage, exposure of invoices, financial loss, and reputational damage |
| Malware Infection | Insufficient shared-computer security | Data theft, file corruption or encryption, business disruption, and recovery costs |
| Unauthorized Network Access | Poorly secured Wi-Fi router | Unauthorized access to connected devices, data theft, account compromise, or service disruption |

---

# 5. SECURITY RECOMMENDATIONS

### 1. Enable Multi-Factor Authentication (MFA)

Enable MFA for employee email and cloud storage to reduce the impact of stolen passwords.

**Mapped Risk:** Phishing + Weak/Reused Passwords

### 2. Use Strong and Unique Passwords

Require strong, unique passwords and use a password manager to reduce password reuse.

**Mapped Risk:** Phishing + Weak/Reused Passwords

### 3. Improve Shared Computer Security

Create separate user accounts, enable automatic screen locking, and restrict unauthorized software installation.

**Mapped Risk:** Malware + Insufficient Computer Security

### 4. Keep Systems and Security Software Updated

Regularly update operating systems, browsers, applications, and antivirus/endpoint security software.

**Mapped Risk:** Malware + Insufficient Computer Security

### 5. Secure the Wi-Fi Router

Change default administrator credentials, use modern Wi-Fi encryption, update router firmware, and disable unnecessary services.

**Mapped Risk:** Unauthorized Network Access + Poorly Secured Router

### 6. Separate Public and Business Network Access

Use a guest network or network segmentation so public Wi-Fi users cannot directly access company devices.

**Mapped Risk:** Unauthorized Network Access + Poorly Secured Router

### 7. Conduct Phishing Awareness Training

Train employees to identify suspicious emails, attachments, links, and fake login pages.

**Mapped Risk:** Phishing + Weak/Reused Passwords

---

## 🔄 Risk Assessment Flow

```text
ASSET
  ↓
THREAT
  ↓
VULNERABILITY
  ↓
RISK / IMPACT
  ↓
SECURITY RECOMMENDATION
