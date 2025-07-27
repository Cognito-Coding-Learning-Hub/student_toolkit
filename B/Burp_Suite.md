# Burp Suite

**Category:** Red Team – Web Application Security  
**Description:**  
Burp Suite is an integrated platform for performing security testing of web applications. It includes tools like a proxy server, spider, repeater, and intruder.

## Key Features
- Intercept and modify HTTP(S) requests
- Automated scanning for vulnerabilities
- Fuzzing with Intruder

## Commands & Tips
- **Start Burp Suite (Community Edition):**
```bash
burpsuite

    Set browser proxy:
    Configure your browser to use 127.0.0.1:8080 as HTTP/HTTPS proxy.

    Common usage:

    Intercept traffic with Proxy tab.

    Send requests to Intruder for fuzzing.

    Analyze responses and adjust payloads.


## Common Steps
- Intercept -> Repeater -> Intruder
