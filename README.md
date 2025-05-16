# 🛡 Web Application Vulnerability Assessment Report

This project demonstrates a **Web Application Vulnerability Assessment** performed as part of my **college project**. The aim was to evaluate and identify potential security issues in web applications using ethical hacking techniques. Two target applications were assessed:

* [Demo Test Fire](https://demotestfire.net)
* [Christhujyothi.com](https://christhujyothi.com)

The assessment followed responsible disclosure practices and was conducted with the required permissions.

---

🔧 **Tools Used**

* **Burp Suite**
* **DirBuster**
* **SQLMap**
* **OWASP ZAP**
* **WhatWeb**

---

🧠 **Testing Methodology**

1. **Information Gathering:** Identified technologies and potential entry points.
2. **Scanning & Enumeration:** Conducted directory brute-forcing, port scanning, and tech stack fingerprinting.
3. **Vulnerability Detection:** Used both manual and automated tools to find vulnerabilities like XSS and SQL Injection.
4. **Exploitation:** Verified findings through safe proof-of-concept testing.
5. **Reporting:** Documented all issues clearly along with remediation suggestions.

---

📘 **Vulnerabilities Identified**

### 1. Reflected XSS (Cross-Site Scripting)

* **Type:** Reflected XSS
* **Affected URL(s):** Input fields that did not sanitize user-supplied data
* **Impact:** Could allow attackers to inject scripts and affect users' browsers

### 2. SQL Injection

* **Type:** Classic SQL Injection
* **Affected URL(s):** Found in login and search functionality
* **Impact:** Attackers could manipulate database queries to bypass authentication or extract data

---

🌐 **Site-wise Summary**

### [Demo Test Fire](https://demotestfire.net)

* ✅ Reflected XSS vulnerability on the login page
* ✅ SQL Injection in the login and product search functions

### [Christhujyothi.com](https://christhujyothi.com)

* ✅ Reflected XSS vulnerability in the contact form

---

🎯 **Recommendations**

* **Input Validation & Output Encoding:** Sanitize and validate all input.
* **Parameterized Queries:** Use secure coding practices to prevent SQL injection.
* **Web Application Firewall (WAF):** Add protection layers for incoming traffic.
* **Security Headers:** Implement CSP, X-Frame-Options, and others for hardening.

---

📌 **Disclaimer**

> This assessment was conducted purely for **educational purposes**, with **prior authorization** from the respective administrators. It aligns with ethical hacking and responsible disclosure policies.
