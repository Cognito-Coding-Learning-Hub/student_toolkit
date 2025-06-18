📘 R → RDP / xRDP / X Server Cheat Sheet
🔧 Install xRDP and Xfce Desktop (Kali/Ubuntu)

sudo apt update && sudo apt install xrdp xfce4 xfce4-goodies -y
sudo systemctl enable xrdp
sudo systemctl start xrdp

🖥️ Set XFCE as default session:

echo "startxfce4" > ~/.xsession

If using a different user:

sudo su - <username> -c 'echo "startxfce4" > ~/.xsession'

🔄 Restart xRDP

sudo systemctl restart xrdp

🛜 Connect from Windows/Linux RDP client

    RDP Address: IP:3389

    Login with your Linux username/password

🛠️ Firewall (if needed)

sudo ufw allow 3389/tcp

🧩 Common Issues

    Black screen? Ensure .xsession exists, and try restarting xrdp + xorg

    Multiple sessions error? Kill stuck sessions:

sudo loginctl terminate-user <username>
