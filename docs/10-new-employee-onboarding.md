# SOP-010: New Employee IT Onboarding

**Category:** Account Management  
**Tier:** 1  
**Average resolution time:** 15–30 minutes

---

## Issue

A new employee is starting and needs their IT accounts, devices, 
and access set up before or on their first day.

---

## Prerequisites

Before starting, confirm the following from HR or the hiring manager:
- Full legal name
- Job title and department
- Start date
- Manager's name
- Required software and systems access
- Whether they need a laptop, desktop, or are BYOD

---

## Step-by-step resolution

### Step 1 — Create the user account

1. Open Active Directory Users and Computers
2. Navigate to the correct department OU
3. Right-click → **New → User**
4. Fill in:
   - First name, last name
   - Username format per company policy (e.g. `firstname.lastname`)
   - Email address
5. Set a temporary password meeting complexity requirements
6. Check **User must change password at next logon**
7. Click **Finish**

### Step 2 — Add user to appropriate security groups

1. Double-click the new user account → **Member Of** tab
2. Click **Add** → add groups based on their role:
   - All staff: `All-Users`, `VPN-Users`
   - IT department: `IT-Admins`
   - Finance: `Finance-Read`, `Finance-Write`
3. Click **OK** to save

### Step 3 — Set up email

1. Assign a mailbox in Microsoft 365 Admin Center
2. Send a welcome email to their personal email with:
   - Their work email address
   - Temporary password
   - IT helpdesk contact information
   - Link to company intranet

### Step 4 — Prepare the device

1. Ensure the device is joined to the domain
2. Install required software per the department's standard 
   software list
3. Install and configure VPN client
4. Install Microsoft 365 apps and sign in with new credentials
5. Configure Outlook with the user's mailbox
6. Run Windows Update and install all pending updates
7. Install any department-specific software requested by manager

### Step 5 — First day verification

1. Meet with the new employee on their first day
2. Have them log in with their temporary password and set a new one
3. Confirm they can access:
   - Email (Outlook)
   - Company intranet
   - VPN (if remote or hybrid)
   - Any department-specific systems
4. Provide them with the IT helpdesk contact information
5. Document the completed onboarding in the ticketing system

---

## Escalation criteria

Escalate to Tier 2 if:
- Specialized software licensing is required
- User needs admin rights on their machine
- Access to sensitive systems requires security team approval
- Device needs to be enrolled in Mobile Device Management (MDM)

---

## Notes

New employee onboarding sets the tone for the employee's 
experience with IT. Always follow up on the first day to 
confirm everything is working a 5-minute check-in prevents 
hours of frustration for the new hire.
