# Security Findings

## SQL Injection

### Description
The login endpoint was vulnerable to SQL Injection.

### Affected Endpoint
POST /rest/user/login

### Payload Used
' OR 1=1 --

### Impact
- Authentication bypass
- Database extraction possible

### Risk Level
High

### Evidence
(Screenshot reference here)

### Recommendation
- Use prepared statements
- Implement input validation
- Use ORM frameworks

---

## 2. Cross-Site Scripting (XSS)

### Description
User input was reflected without sanitization.

### Payload Used
<script>alert(1)</script>

### Impact
- Session hijacking
- Cookie theft
- Malicious script execution

### Risk Level
Medium

### Evidence
(Screenshot reference here)

### Recommendation
- Encode output
- Implement CSP headers
- Sanitize user input

---

## 3. Cross-Site Request Forgery (CSRF)

### Description
Sensitive action lacked CSRF token validation.

### Affected Function
Password Change

### Impact
- Unauthorized action execution

### Risk Level
Medium

### Recommendation
- Implement anti-CSRF tokens
- Use SameSite cookie attribute
