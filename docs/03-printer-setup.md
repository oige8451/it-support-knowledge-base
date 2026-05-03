# SOP-003: Printer Setup and Troubleshooting

**Category:** Hardware & Peripherals  
**Tier:** 1  
**Average resolution time:** 5–10 minutes

---

## Issue

User is unable to print, cannot find the printer, or needs a 
printer set up on their workstation.

---

## Possible causes

- Printer driver not installed on user's machine
- User connected to wrong network or VPN (network printers 
  won't appear off-network)
- Printer is offline or out of paper/ink
- Print spooler service has stopped on user's machine
- User does not have permission to access the printer

---

## Step-by-step resolution

### Scenario A — Printer not showing up

1. Confirm user is connected to the correct network (not VPN 
   if printer is local)
2. Go to **Settings → Bluetooth & devices → Printers & scanners**
3. Click **Add a printer or scanner**
4. If printer appears in the list → click it → click **Add device**
5. If printer does not appear → click **The printer I want isn't 
   listed** → enter the printer's IP address manually
6. Install the driver if prompted — download from manufacturer's 
   website if needed
7. Print a test page to confirm

### Scenario B — Printer shows as offline

1. Check the physical printer — power, paper, ink/toner
2. Go to **Settings → Printers & scanners** → click the printer
3. Click **Open print queue**
4. Click **Printer** in the menu → uncheck **Use Printer Offline**
5. If still offline, restart the Print Spooler service:
   - Press **Win + R** → type `services.msc` → press Enter
   - Find **Print Spooler** → right-click → **Restart**
6. Try printing again

### Scenario C — Print jobs stuck in queue

1. Open **Settings → Printers & scanners** → click the printer
2. Click **Open print queue**
3. Select all stuck jobs → press **Delete**
4. If jobs won't delete, restart the Print Spooler service 
   (see Scenario B step 5)
5. Try printing again after clearing the queue

---

## Escalation criteria

Escalate to Tier 2 if:
- Driver installation fails repeatedly
- Printer requires network configuration changes
- User needs access permissions added to a shared printer
- Issue affects multiple users on the same printer

---

## Notes

Always check the physical printer first before troubleshooting 
software — most printer calls are resolved by checking paper 
tray, ink levels, or power cable.
