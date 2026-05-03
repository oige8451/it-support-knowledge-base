# SOP-005: VPN Setup and Troubleshooting

**Category:** Network & Connectivity  
**Tier:** 1  
**Average resolution time:** 5–10 minutes

---

## Issue

User is unable to connect to VPN, needs VPN set up on their 
device, or reports VPN dropping frequently.

---

## Possible causes

- VPN client not installed or outdated
- User credentials expired or incorrect
- Multi-factor authentication (MFA) not completing
- Firewall or antivirus blocking VPN connection
- User connecting from a network that blocks VPN ports
- VPN server outage affecting all users

---

## Step-by-step resolution

### Scenario A — VPN not installed

1. Confirm which VPN client your organization uses
2. Direct user to the company intranet or IT portal to download 
   the approved VPN client
3. Walk user through installation:
   - Download the installer
   - Run as Administrator
   - Accept defaults unless IT policy specifies otherwise
4. Once installed, provide the VPN server address
5. User logs in with their domain credentials
6. Test connection by accessing an internal resource

### Scenario B — VPN installed but won't connect

1. Confirm user credentials are correct — test by logging into 
   another company system with the same credentials
2. Check if MFA prompt appeared and was completed correctly
3. Disconnect any other VPN or proxy software running 
   simultaneously
4. Temporarily disable antivirus → attempt connection → 
   re-enable antivirus after testing
5. Uninstall and reinstall the VPN client if above steps fail
6. Ask user to try connecting from a different network 
   (e.g. phone hotspot) to rule out network blocking

### Scenario C — VPN connects but drops frequently

1. Ask user to check their internet connection stability first
2. Check VPN client for an auto-reconnect setting → enable it
3. Update the VPN client to the latest version
4. Check if issue occurs on other networks — if only on home 
   network, ISP may be throttling VPN traffic
5. Log the frequency and timing of drops for Tier 2 escalation 
   if issue persists

---

## Escalation criteria

Escalate to Tier 2 if:
- VPN server address or configuration needs to be changed
- User account needs VPN access permissions granted
- Multiple users cannot connect simultaneously
- Certificate errors appear during connection
- Issue persists after full reinstall

---

## Notes

Never troubleshoot VPN issues by asking users to disable their 
firewall permanently — only disable temporarily for testing and 
always confirm it is re-enabled afterward. VPN access is a 
security boundary and any suspected unauthorized access attempts 
should be flagged to the security team immediately.
