🐧 Linux Must-Know Command Cheat Sheet
📂 Navigation & Files

pwd                # Show current directory
ls                 # List files
ls -la             # List all files (including hidden) with details
cd /path/to/dir    # Change directory
cd ~               # Go to home directory
cd ..              # Move up one directory
tree               # View directory tree (install with `sudo apt install tree`)

📄 Viewing Files

cat file.txt       # View file contents
less file.txt      # View file page by page (q to quit)
head file.txt      # Show first 10 lines
tail file.txt      # Show last 10 lines
tail -f file.log   # Live follow a growing log file
wc -l file.txt     # Count lines

✏️ Creating & Editing Files

touch file.txt     # Create empty file
nano file.txt      # Edit file in Nano
vim file.txt       # Edit file in Vim
cp file1 file2     # Copy file
mv file1 file2     # Move or rename file
rm file.txt        # Delete file
mkdir newdir       # Create new directory
rm -r dir          # Delete directory and contents

🔍 Searching

find /path -name filename       # Find files by name
grep "pattern" file.txt         # Search for pattern in file
grep -R "pattern" /path         # Recursive search
locate filename                 # Quickly find files (updatedb first)

📦 Permissions

ls -l               # View file permissions
chmod 755 script.sh # Change permissions (rwxr-xr-x)
chmod +x script.sh  # Make file executable
chown user:group file.txt # Change owner

⚡ Processes & System

top                # Show running processes (q to quit)
htop               # Interactive process viewer (install if needed)
ps aux             # Detailed process list
kill 1234          # Kill process by PID
killall name       # Kill process by name
uptime             # Show system uptime
whoami             # Show current user
id                 # Show user and group info

🌐 Networking

ifconfig           # Show network interfaces (or `ip addr`)
ping 8.8.8.8       # Ping a host
netstat -tulnp     # Show listening ports (or `ss -tulnp`)
curl example.com   # Fetch web page
wget http://url    # Download a file
scp file user@host:/path # Copy file to remote host
ssh user@host      # Connect to remote host via SSH

🔧 Package Management

Debian/Ubuntu:

sudo apt update              # Update package list
sudo apt upgrade             # Upgrade installed packages
sudo apt install packagename # Install package
sudo apt remove packagename  # Remove package

RHEL/CentOS:

sudo yum install packagename
sudo dnf install packagename

💡 Disk & Storage

df -h             # Show disk usage
du -sh folder/    # Show folder size
mount | grep /mnt # View mounts
lsblk             # List block devices
fdisk -l          # Show disk partitions

🧰 User Management

adduser newuser   # Add user
passwd newuser    # Change password
usermod -aG sudo username # Add user to sudo group
who               # Show logged-in users

🔐 Archive & Compression

tar -czvf file.tar.gz folder/  # Compress folder
tar -xzvf file.tar.gz          # Extract tar.gz
zip -r file.zip folder/        # Zip folder
unzip file.zip                 # Unzip

✨ Tips

✅ Use man command to get help for any command
✅ Use --help with a command to see options (e.g., ls --help)
✅ Combine commands with | (pipe) to chain outputs (ls -l | grep txt)
