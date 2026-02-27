# Testing Methodology

## Approaching the Target 
The assessment was conducted using a black-box testing methodology.Black-box testing is
a software testing method that verifies functionality against specifications without examining internal code or structure. 

## Stages of web application penetration testing

### Stage 1: Reconnaissance (Skipped Cause this is tested within the localhost)
- Identifing the Web application 
- Mapped attack surface using fuff, gobuster ,dir.

### Stage 2: Interception
- Captured HTTP requests using Burp Suite
- Analyzed parameters and input fields

### Stage 3: Vulnerability Testing

#### SQL Injection Testing
- Identified input fields
- Tested manual payloads
- Automated testing using SQLMap

#### Cross-Site Scripting (XSS)
- Tested reflected input fields
- Injected JavaScript payloads
- Verified execution in browser and alert showed (Confirmed XSS)

#### Cross-Site Request Forgery (CSRF)
- Analyzed sensitive actions
- Checked for CSRF tokens
- Tested request replay

### Phase 4: Automated Scanning
- Conducted scan using OWASP ZAP
- Analyzed alerts and severity levels

## 3. Risk Classification
Based on impact and exploitability:
- High
- Medium
- Low
