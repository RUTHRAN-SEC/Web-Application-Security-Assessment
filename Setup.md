# Setup Documentation

## Goal
To set up a controlled environment for performing a web application security assessment.

## Environment Details
- Operating System:Kali GNU/Linux Rolling
- RAM:8GB
- Browser: FireFox
- Target Application: OWASP Juice Shop
- Hosting Method: Docker in localhost

## Tools Installed
- Burp Suite
- OWASP ZAP
- SQLMap
- Docker

## Installation Steps for OWASP Juice Shop using docker(Linux)

### Install Docker
Commands used:
```
docker pull bkimminich/juice-shop
```


### Pull OWASP Juice Shop
Commands used:
```
docker pull bkimminich/juice-shop
```

### Run OWASP Juice Shop in localhost
Command used:
```
docker run --rm -p 127.0.0.1:3000:3000 bkimminich/juice-shop
```

### Configure Burp Suite Proxy
- Proxy IP: 127.0.0.1
- Port: 8080
- Browser Configuration: Install FoxyProxy Basic and Add CA certificate

## Scope of the Target
Target URL: http://localhost:3000
Tested in safe environment 
