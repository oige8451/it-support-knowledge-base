# SOP-004: Wi-Fi and Network Connectivity Troubleshooting

**Category:** Network & Connectivity  
**Tier:** 1  
**Average resolution time:** 5–10 minutes

---

## Issue

User reports no internet access, slow connection, or inability 
to connect to the company Wi-Fi network.

---

## Possible causes

- Wi-Fi adapter disabled on user's device
- User connected to wrong network (personal hotspot vs corporate)
- IP address conflict on the network
- DNS server not responding
- Network adapter driver issue
- Router or access point issue affecting multiple users

---

## Step-by-step resolution

### Step 1 — Check the basics first

1. Confirm Wi-Fi is turned on — check the taskbar Wi-Fi icon
2. Ask if other devices in the same location have internet access
   - If yes → issue is isolated to this device
   - If no → possible network outage, escalate immediately
3. Ask if the issue started after any recent changes (Windows 
   update, new software, moving to a different office)

### Step 2 — Reconnect to the network

1. Click the Wi-Fi icon in the taskbar
2. Click the arrow next to the company network
3. Click **Disconnect** → wait 10 seconds → click **Connect**
4. Test internet access

### Step 3 — Run the built-in troubleshooter

1. Go to **Settings → System → Troubleshoot → Other troubleshooters**
2. Click **Run** next to **Internet Connections**
3. Follow the prompts and apply any fixes suggested
4. Test internet access again

### Step 4 — Flush DNS and renew IP address

1. Press **Win + R** → type `cmd` → press Enter
2. Type the following commands one at a time:
netsh winsock reset
netsh int ip reset
ipconfig /release
ipconfig /flushdns
ipconfig /renew
3. Restart the computer
4. Test internet access

### Step 5 — Check network adapter

1. Right-click Start → **Device Manager**
2. Expand **Network Adapters**
3. Look for any yellow warning icons
4. If found → right-click the adapter → **Update driver**
5. Restart and test

---

## Escalation criteria

Escalate to Tier 2 if:
- Multiple users in the same area are affected
- Issue persists after all steps above
- Device manager shows adapter errors that won't resolve
- User needs access to a specific network VLAN or SSID

---

## Notes

Always ask "is anyone else affected?" first — if multiple users 
are down it's a network infrastructure issue and should be 
escalated immediately rather than troubleshooting individual devices.
