# ApexPlanet Internship – Task 3
## Web Application Security Testing and Assessment

### Objective
The objective of this task was to understand common web application vulnerabilities, perform security testing in a controlled lab environment, analyze application behavior, and document findings along with mitigation techniques.

---

## Environment Setup

- Kali Linux 2025
- DVWA (Damn Vulnerable Web Application)
- Apache Web Server
- Burp Suite Community Edition
- Firefox Browser
- SecurityHeaders.com
- VirtualBox Lab Environment

---

## Modules Covered

### 1. SQL Injection (SQLi)

SQL Injection testing was performed on DVWA to understand how improper input validation can allow attackers to manipulate database queries.

**Activities Performed**
- Tested normal user input.
- Executed SQL Injection payloads.
- Retrieved additional database records.
- Observed insecure query execution.

**Mitigation**
- Parameterized Queries (Prepared Statements)
- Input Validation
- Stored Procedures
- Least Privilege Database Accounts

---

### 2. Cross-Site Scripting (XSS)

Reflected and Stored XSS vulnerabilities were tested to demonstrate how malicious scripts can execute within a victim's browser.

**Activities Performed**
- Injected JavaScript payloads.
- Triggered alert popups.
- Tested reflected and stored attack scenarios.
- Analyzed browser behavior.

**Mitigation**
- Input Sanitization
- Output Encoding
- Content Security Policy (CSP)
- HttpOnly Cookies

---

### 3. Cross-Site Request Forgery (CSRF)

CSRF attacks were demonstrated to understand how authenticated users can unknowingly perform actions on behalf of attackers.

**Activities Performed**
- Created a malicious CSRF request.
- Executed unauthorized actions.
- Enabled CSRF protection mechanisms.
- Verified token validation.

**Mitigation**
- CSRF Tokens
- SameSite Cookies
- Origin Validation
- User Re-authentication for Sensitive Actions

---

### 4. File Inclusion Attacks

Local File Inclusion (LFI) and Remote File Inclusion (RFI) concepts were explored using DVWA.

**Activities Performed**
- Accessed local system files.
- Tested file inclusion behavior.
- Observed PHP security restrictions.
- Analyzed application responses.

**Mitigation**
- Input Validation
- Whitelisting
- Disable Remote File Inclusion
- Restrict File Access Permissions

---

### 5. Burp Suite Advanced Testing

Burp Suite was used to intercept, modify, and analyze HTTP requests and responses.

**Activities Performed**
- Configured FoxyProxy.
- Captured login requests.
- Modified request parameters.
- Used Burp Intruder for fuzzing.
- Compared response lengths and status codes.

**Mitigation**
- Strong Authentication Controls
- Rate Limiting
- Account Lockout Policies
- Secure Session Management

---

### 6. Web Security Headers

HTTP Security Headers were analyzed and implemented to improve browser-side security.

**Activities Performed**
- Evaluated security headers using SecurityHeaders.com.
- Enabled Apache Headers Module.
- Configured security-related headers.
- Verified implementation using HTTP response inspection.

**Implemented Headers**
- X-Frame-Options
- X-Content-Type-Options
- Referrer-Policy
- X-XSS-Protection

**Mitigation Benefits**
- Clickjacking Protection
- MIME-Type Sniffing Prevention
- Referrer Information Control
- Browser-Based XSS Protection

---

## Key Learning Outcomes

Through this task, the following concepts were learned:

- Web Application Vulnerability Assessment
- SQL Injection Exploitation Techniques
- Cross-Site Scripting Attacks
- Cross-Site Request Forgery Attacks
- File Inclusion Vulnerabilities
- HTTP Request Interception
- Burp Suite Usage
- Security Header Implementation
- Secure Coding Practices
- Web Application Hardening Techniques

---

## Conclusion

This task provided practical exposure to identifying, exploiting, and mitigating common web application vulnerabilities in a controlled laboratory environment. The exercises demonstrated the importance of secure coding practices, proper input validation, security headers, and defense-in-depth strategies for protecting modern web applications.

---

### Internship
**ApexPlanet Software Pvt. Ltd.**

**Domain:** Cyber Security & Ethical Hacking

**Task:** Web Application Security Testing and Assessment
