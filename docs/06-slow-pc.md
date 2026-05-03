# SOP-006: Slow PC Performance

**Category:** Software & OS  
**Tier:** 1  
**Average resolution time:** 10–15 minutes

---

## Issue

User reports their computer is running slowly, freezing, or 
taking a long time to start up or open applications.

---

## Possible causes

- Too many programs running at startup
- Low disk space (less than 10% free)
- Malware or virus infection
- Outdated drivers or Windows updates pending
- Insufficient RAM for current workload
- Hard drive failing (older machines)

---

## Step-by-step resolution

### Step 1 — Check current resource usage

1. Press **Ctrl + Shift + Esc** to open Task Manager
2. Click the **Performance** tab
3. Check CPU, Memory, and Disk usage
   - CPU consistently above 90% → identify the process using it
   - Memory above 90% → too many applications open
   - Disk at 100% → common on older machines with HDDs
4. Click the **Processes** tab → sort by CPU or Memory → 
   identify any unusual processes using high resources
5. If an unknown process is using high resources → flag for 
   malware scan before proceeding

### Step 2 — Disable unnecessary startup programs

1. In Task Manager → click **Startup apps** tab
2. Review all enabled startup programs
3. Right-click any non-essential programs → **Disable**
   - Keep: antivirus, corporate security tools
   - Disable: Spotify, Teams (if not required at startup), 
     OneDrive (if not required)
4. Restart the computer and test

### Step 3 — Free up disk space

1. Press **Win + R** → type `cleanmgr` → press Enter
2. Select the C: drive → click OK
3. Check all boxes → click **Clean up system files**
4. Also check C: drive free space:
   - Open File Explorer → right-click C: drive → Properties
   - If less than 10% free → advise user on large file cleanup
   - Move large files to network storage or external drive

### Step 4 — Run Windows Update

1. Go to **Settings → Windows Update**
2. Click **Check for updates**
3. Install all pending updates
4. Restart if required
5. Test performance after restart

### Step 5 — Run a malware scan

1. Open **Windows Security** from the Start menu
2. Click **Virus & threat protection**
3. Click **Quick scan**
4. If threats found → click **Remove** → restart → run full scan

---

## Escalation criteria

Escalate to Tier 2 if:
- Task Manager shows unknown processes with high resource usage 
  that persist after malware scan
- Disk is showing errors in Event Viewer
- RAM upgrade or hardware replacement may be needed
- Issue affects multiple machines simultaneously

---

## Notes

Always check Task Manager first before making any changes — 
it gives you the fastest picture of what is actually causing 
the slowdown and prevents unnecessary steps.
