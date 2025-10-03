# 🔧 Firewall Configuration Guide

## 🖥️ Windows Firewall Setup

### Step 1: Access Windows Firewall
1. Open Windows Security
2. Go to "Firewall & network protection"
3. Click "Advanced settings" for Windows Defender Firewall

### Step 2: View Current Rules
- Inbound Rules: 100+ rules typically present
- Outbound Rules: 80+ rules typically present
- Default: Most inbound traffic blocked, outbound allowed

### Step 3: Block Telnet (Port 23)
1. Click "Inbound Rules" → "New Rule"
2. Select "Port" → Click "Next"
3. Select "TCP" and enter "23" in "Specific local ports"
4. Select "Block the connection" → Click "Next"
5. Apply to all profiles (Domain, Private, Public) → Click "Next"
6. Name: "Block Telnet Port 23" → Click "Finish"

### Step 4: Test the Block Rule
```cmd
telnet localhost 23
