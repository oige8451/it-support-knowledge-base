# SOP-002: Account Lockout

**Category:** Account Management  
**Tier:** 1  
**Average resolution time:** 3–5 minutes

---

## Issue

User receives an error stating their account has been locked out 
and cannot log in.

---

## Possible causes

- Too many failed login attempts (default threshold: 5 attempts)
- User typing password incorrectly (caps lock, keyboard language)
- Cached credentials on another device still attempting to 
  authenticate with old password
- Malicious login attempts (flag for security team if repeated)

---

## Step-by-step resolution

1. Verify the user's identity before making any changes
2. Ask the user if they recently changed their password — 
   old credentials on phones or other devices often cause 
   repeated lockouts
3. Navigate to the user account in Active Directory Users 
   and Computers
4. Double-click the user → go to the **Account** tab
5. Check if **Unlock account** checkbox is ticked — if yes, 
   check it to unlock
6. Click **OK** to save
7. Ask the user to check all devices (phone, tablet, home PC) 
   and update saved passwords
8. Ask the user to attempt login and confirm success
9. Log the resolution in the ticketing system

---

## Escalation criteria

Escalate to Tier 2 or flag to security team if:
- Account is locking out repeatedly within minutes of being unlocked
- Multiple accounts locking out simultaneously
- Suspected brute force or unauthorized access attempt

---

## Notes

Repeated lockouts from a single account within a short period 
should always be flagged to the security team as a potential 
security incident — do not just keep unlocking without investigating.
