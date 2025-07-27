🟥 Red Team Tools (Offensive)
Tool	Example Commands	What It Does
Nmap	nmap -sV -p- 10.10.10.1	Network scanner, discovers hosts, services, versions.  
Metasploit Framework	msfconsole → use exploit/multi/handler	Exploitation framework for known vulnerabilities.  
Nikto	nikto -h http://target.com	Web server scanner for vulnerabilities and misconfigurations.  
Hydra	hydra -l admin -P passwords.txt 10.10.10.5 ssh	Brute-force login for many protocols (SSH, FTP, RDP, etc.).  
Burp Suite	Proxy browser through Burp → Intercept	Web app testing: intercept, modify, and replay requests.  
Gobuster	gobuster dir -u http://target -w /usr/share/wordlists/dirb/common.txt	Directory and file brute forcing on webservers.  
SQLmap	sqlmap -u "http://target/item?id=1" --dbs	Automated SQL injection and database dumping.  
John the Ripper	john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt	Password hash cracker.  
Aircrack-ng	airmon-ng start wlan0 → airodump-ng wlan0mon	Wireless network cracking and sniffing.  
Responder	responder -I eth0	Captures NTLM/LM hashes via rogue services on the network.  
🟦 Blue Team Tools (Defensive)  
Tool	Example Commands	What It Does  
Wireshark	wireshark (GUI)	Packet capture and deep network protocol analysis.  
Tcpdump	tcpdump -i eth0 -w capture.pcap	Command-line packet sniffer.  
OSSEC/Wazuh	Runs as agent	Host-based intrusion detection and log monitoring.  
Lynis	lynis audit system	Security auditing tool for Linux systems.  
Chkrootkit	chkrootkit	Detects known rootkits on a system.  
RKHunter	rkhunter --check	Scans for rootkits, backdoors, and local exploits.  
ClamAV	clamscan -r /home/user	Open-source antivirus scanner.  
Fail2Ban	fail2ban-client status	Bans IPs that show malicious signs in logs (e.g., failed logins).  
Snort	snort -A console -i eth0 -c /etc/snort/snort.conf	Network intrusion detection and prevention system.  
OpenVAS/Greenbone	openvas-check-setup	Full vulnerability scanning platform for defense posture.  
✨ Example Scenarios

🔴 Red Team (Attacker’s POV):

    Recon target:
    nmap -A 192.168.1.0/24

    Brute-force SSH:
    hydra -l root -P /usr/share/wordlists/rockyou.txt 192.168.1.10 ssh

🔵 Blue Team (Defender’s POV):

    Investigate suspicious network traffic:
    tcpdump -i eth0 host 192.168.1.10

    Audit Linux box for weaknesses:
    lynis audit system
