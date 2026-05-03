# SOP-001: Password Reset

**Category:** Account Management  
**Tier:** 1  
**Average resolution time:** 3–5 minutes

---

## Issue

User is unable to log in and requests a password reset.

---

## Possible causes

- Password has expired (default policy: 90 days)
- User forgot their password
- Account locked after too many failed attempts (handle via SOP-002)

---

## Step-by-step resolution

1. Verify the user's identity — confirm full name and employee ID 
   or department before proceeding
2. Navigate to user account in directory (Active Directory Users 
   and Computers or IT ticketing system)
3. Right-click the user account → **Reset Password**
4. Set a temporary password meeting complexity requirements:
   - Minimum 12 characters
   - Must include uppercase, lowercase, number, and symbol
   - Example format: `Welcome@2024`
5. Check the box **User must change password at next logon**
6. Click **OK** to confirm
7. Inform the user of their temporary password securely — never 
   send passwords via email
8. Ask the user to log in and confirm the password change was 
   successful
9. Log the resolution in the ticketing system with timestamp

---

## Escalation criteria

Escalate to Tier 2 if:
- User account does not exist in the directory
- Reset option is greyed out or unavailable
- User reports being locked out across multiple systems simultaneously

---

## Notes

Never reset a password without verifying identity first. If you 
cannot verify identity, escalate to a supervisor.
