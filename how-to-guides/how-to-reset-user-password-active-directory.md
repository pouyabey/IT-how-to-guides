# How to Reset a User Password in Active Directory

### How I Write How-To Guides

- Review the task and define the purpose
- Identify the audience and required access
- Write clear step-by-step instructions
- Add screenshots for key steps
- Include expected results
- Add common issues and quick fixes
- Write verification steps
- Add escalation notes if needed
- Keep the guide simple and easy to update

---

## Purpose
This guide explains how to reset a user password in Active Directory Users and Computers and confirm the account is ready for login.

## Audience
IT support technicians and help desk staff.

## Requirements
- Windows Server or admin workstation
- Active Directory Users and Computers access
- Permission to reset user passwords

---

## Steps

### Step 1: Open Active Directory Users and Computers
Open Server Manager, go to Tools, and select Active Directory Users and Computers.

Screenshot:
![Open Active Directory Users and Computers](screenshots/ad-password-reset-01-open-aduc.png)

Expected result:
Active Directory Users and Computers opens successfully.

---

### Step 2: Find the User Account
Search for the user or browse to the correct Organizational Unit.

Screenshot:
![Find User Account](screenshots/ad-password-reset-02-find-user.png)

Expected result:
The correct user account is located.

---

### Step 3: Reset the Password
Right-click the user account and select Reset Password.

Screenshot:
![Reset Password Option](screenshots/ad-password-reset-03-reset-password.png)

Expected result:
The Reset Password window opens.

---

### Step 4: Enter a Temporary Password
Enter a temporary password, confirm it, and check User must change password at next logon.

Screenshot:
![Enter Temporary Password](screenshots/ad-password-reset-04-temporary-password.png)

Expected result:
The password is reset successfully.

---

### Step 5: Unlock the Account if Needed
If the account is locked, open the user properties and unlock the account.

Screenshot:
![Unlock Account](screenshots/ad-password-reset-05-unlock-account.png)

Expected result:
The user account is unlocked and ready for login.

---

## Verification
Confirm that:
- The password was reset successfully.
- The account is not locked.
- The user can sign in with the temporary password.
- The user changes the password at next logon.

## Common Issues
- User still cannot log in: Confirm the correct username and domain.
- Account locks again: Check for saved old passwords on another device or application.
- Password does not meet requirements: Use a password that meets the domain password policy.

## Documentation Notes
Example ticket note:

User requested a password reset. Verified the user account in Active Directory, reset the password, selected “User must change password at next logon,” checked that the account was not locked, and confirmed the user was able to sign in successfully.
