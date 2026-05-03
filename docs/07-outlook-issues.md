# SOP-007: Outlook Issues

**Category:** Email & Communication  
**Tier:** 1  
**Average resolution time:** 5–10 minutes

---

## Issue

User reports Outlook not opening, emails not sending or 
receiving, or Outlook running slowly.

---

## Possible causes

- Outlook profile corrupted
- Mailbox full or over quota
- Cached data causing sync issues
- Outdated Office installation
- Network connectivity issues affecting Exchange connection

---

## Step-by-step resolution

### Scenario A — Outlook won't open

1. Press **Ctrl + Alt + Delete** → Task Manager
2. Check if Outlook.exe is already running in background
   - If yes → right-click → End Task → reopen Outlook
3. If still won't open → press **Win + R** → type 
   `outlook.exe /safe` → press Enter
   - This opens Outlook in safe mode (no add-ins)
   - If it opens in safe mode → an add-in is the problem
   - Go to **File → Options → Add-ins → Manage COM Add-ins** 
     → disable all → restart Outlook normally → re-enable 
     one by one to find the culprit
4. If safe mode doesn't work → repair Office:
   - Go to **Settings → Apps** → find Microsoft 365
   - Click **Modify → Quick Repair** → follow prompts

### Scenario B — Emails not sending or receiving

1. Check internet connectivity first
2. Look at the bottom of Outlook for connection status:
   - Should say **Connected to Microsoft Exchange**
   - If disconnected → check network → restart Outlook
3. Check if mailbox is full:
   - **File → Info** → check mailbox size
   - If over quota → advise user to delete or archive old emails
4. Send a test email to yourself to confirm sending works
5. Check Junk folder for missing incoming emails

### Scenario C — Outlook running slowly

1. Clear the Outlook cache:
   - Close Outlook
   - Press **Win + R** → type 
     `%localappdata%\Microsoft\Outlook`
   - Delete all `.ost` files (Outlook will rebuild them)
   - Reopen Outlook and allow it to sync
2. Disable unused add-ins (see Scenario A step 3)
3. Reduce mailbox size by archiving old emails:
   - **File → Tools → Clean Up Old Items**

---

## Escalation criteria

Escalate to Tier 2 if:
- Office repair fails to resolve the issue
- User's mailbox needs quota increase
- Outlook profile needs to be rebuilt
- Issue affects multiple users simultaneously

---

## Notes

Never delete .ost files while Outlook is open — always close 
Outlook first. The .ost file rebuilds automatically on next 
launch and this process can take several minutes for large mailboxes.
