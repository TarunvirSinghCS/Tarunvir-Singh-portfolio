# Windows Account Could Not Log In

## Problem
A Windows laptop displayed “The username or password is incorrect” even though I was entering the correct credentials.

## Investigation
- Verified the password by logging into the Microsoft account online.  
- Checked Caps Lock and keyboard layout.  
- Booted into Safe Mode to isolate potential software interference.  
- Checked event logs for authentication errors.

## Solution
The laptop had cached old credentials from a previous domain login. Removing the old cached credentials via Credential Manager and restarting the laptop fixed the login issue.

## What I Learned
- Cached credentials can block logins even with correct passwords.  
- Safe Mode is helpful for isolating login issues.  
- Checking system logs provides clues before more drastic steps.

## What Tools Helped
- Event Viewer  
- Credential Manager  
- Safe Mode login environment  
