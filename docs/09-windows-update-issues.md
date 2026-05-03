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
