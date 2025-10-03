# 🖥️ Windows Firewall Configuration

## 🔧 Step-by-Step Windows Firewall Setup

### Step 1: Access Windows Defender Firewall
1. Press `Windows Key + R`
2. Type `wf.msc` and press Enter
3. Or go to: Control Panel → System and Security → Windows Defender Firewall

### Step 2: View Current Rules
- **Inbound Rules:** Shows rules for incoming traffic
- **Outbound Rules:** Shows rules for outgoing traffic  
- **Monitor:** View active firewall status

### Step 3: Block Telnet Port (23) - INBOUND
1. In Windows Defender Firewall, click "Inbound Rules"
2. Click "New Rule" in the right panel
3. Select "Port" → Click "Next"
4. Select "TCP" and enter "23" in "Specific local ports"
5. Select "Block the connection" → Click "Next"
6. Check all three profiles (Domain, Private, Public) → Click "Next"
7. Name: "Block Telnet Inbound" → Description: "Task 4 - Block Telnet port 23" → Click "Finish"

### Step 4: Test the Block Rule
Open Command Prompt and test:
```cmd
telnet localhost 23
