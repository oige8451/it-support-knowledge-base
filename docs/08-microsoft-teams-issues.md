# SOP-008: Microsoft Teams Issues

**Category:** Email & Communication  
**Tier:** 1  
**Average resolution time:** 5–10 minutes

---

## Issue

User reports Teams not loading, audio or video not working 
in meetings, or messages not sending.

---

## Possible causes

- Teams client needs updating
- Microphone or camera permissions not granted
- Wrong audio device selected in Teams settings
- Teams cache corrupted
- Network or firewall blocking Teams traffic

---

## Step-by-step resolution

### Scenario A — Teams not loading or crashing

1. Close Teams completely:
   - Right-click Teams icon in system tray → **Quit**
2. Clear Teams cache:
   - Press **Win + R** → type `%appdata%\Microsoft\Teams`
   - Delete the contents of these folders:
     - `Cache`
     - `blob_storage`
     - `databases`
     - `Local Storage`
   - Do not delete the folders themselves, only contents
3. Reopen Teams and test

### Scenario B — Audio or video not working in meetings

1. Before the meeting → click your profile picture in Teams
   → **Settings → Devices**
2. Confirm correct microphone and speaker are selected
3. Click **Make a test call** to verify audio works
4. If camera not showing:
   - Check camera privacy settings:
     **Settings → Privacy → Camera** → ensure Teams is allowed
   - Check if another application is using the camera 
     simultaneously
5. If using external headset → unplug and replug → 
   reselect in Teams device settings

### Scenario C — Messages not sending

1. Check internet connectivity
2. Check Teams status at **status.office.com** — confirm 
   no Microsoft outage
3. Sign out of Teams → sign back in:
   - Click profile picture → **Sign out**
   - Sign back in with domain credentials
4. If issue persists → clear cache (see Scenario A step 2)

---

## Escalation criteria

Escalate to Tier 2 if:
- User cannot sign in despite correct credentials
- Teams is blocked by corporate firewall
- Issue affects all users in the organization simultaneously
- User needs guest access or external collaboration configured

---

## Notes

Always check status.office.com before spending time 
troubleshooting Teams issues — if Microsoft is having a service 
outage, no amount of local troubleshooting will fix it. Inform 
the user and set expectations accordingly.
