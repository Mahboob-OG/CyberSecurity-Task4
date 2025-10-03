# CyberSecurity-Task4
# 🔥 Task 4: Setup and Use a Firewall on Windows/Linux

## 📌 Objective
Configure and test basic firewall rules to allow or block network traffic using Windows Firewall or UFW (Uncomplicated Firewall) on Linux.

## 🛠️ Tools Used
- **Windows:** Windows Defender Firewall
- **Linux:** UFW (Uncomplicated Firewall)
- **Testing Tools:** telnet, ping, netstat

## 🎯 Tasks Completed
1. Listed current firewall rules
2. Created inbound rule to block Telnet (port 23)
3. Tested the block rule using telnet command
4. Created allow rule for SSH (port 22) on Linux
5. Removed test rules to restore original state
6. Documented all steps and commands

## 📁 Files Included
- `firewall_configuration.md` - Detailed configuration steps
- `firewall_concepts.md` - Firewall concepts and interview answers
- `screenshots/` - Firewall rules and testing evidence

## 🔧 Commands Used (Linux UFW)
```bash
sudo ufw status verbose
sudo ufw deny 23/tcp
sudo ufw allow 22/tcp
sudo ufw delete deny 23/tcp
