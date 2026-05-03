# SOP-009: Windows Update Issues

**Category:** Software & OS  
**Tier:** 1  
**Average resolution time:** 10–15 minutes

---

## Issue

User reports Windows updates failing to install, getting stuck, 
or receiving error codes during the update process.

---

## Possible causes

- Windows Update service not running
- Corrupted update cache
- Insufficient disk space for update
- Conflicting software blocking the update
- Update requires a restart that has been postponed too long

---

## Step-by-step resolution

### Step 1 — Check disk space first

1. Open File Explorer → right-click C: drive → Properties
2. Windows updates require at least **10 GB free space**
3. If low → run Disk Cleanup before proceeding:
   - Press **Win + R** → type `cleanmgr` → press Enter
   - Check all boxes → **Clean up system files** → OK

### Step 2 — Run the Windows Update troubleshooter

1. Go to **Settings → System → Troubleshoot → 
   Other troubleshooters**
2. Click **Run** next to **Windows Update**
3. Apply any fixes suggested
4. Go to **Settings → Windows Update → Check for updates**
5. Test if updates now install

### Step 3 — Reset Windows Update components

1. Press **Win + R** → type `cmd` → 
   right-click → **Run as administrator**
2. Type these commands one at a time pressing Enter after each:
      net stop wuauserv
      net stop cryptSvc
      net stop bits
      net stop msiserver
      ren C:\Windows\SoftwareDistribution SoftwareDistribution.old
      net start wuauserv
      net start cryptSvc
      net start bits
      net start msiserver
3. Restart the computer
4. Go to **Settings → Windows Update → Check for updates**
5. Updates should now download and install fresh

### Step 4 — Install updates manually

1. Note the error code shown in Windows Update
2. Go to **catalog.update.microsoft.com**
3. Search for the update using its KB number 
   (shown in update details)
4. Download and install manually
5. Restart and verify

---

## Escalation criteria

Escalate to Tier 2 if:
- Error persists after resetting update components
- Update is required for security compliance and cannot wait
- System restore may be needed after a failed update
- Update is being blocked by Group Policy

---

## Notes

Always note the exact error code before troubleshooting — 
Microsoft's support site has specific fixes for each error code 
which can save significant troubleshooting time.
