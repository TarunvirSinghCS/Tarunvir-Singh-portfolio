# What Happens When a User Logs Into a Computer

## Overview
Logging into a computer involves verifying a user’s identity so they can securely access files, applications, and system resources. This process includes input validation, authentication, and session creation to ensure the correct user gains access.

## Steps
1. **User enters credentials** – Typically a username and password, sometimes combined with a second factor.  
2. **Credentials sent to authentication system** – Input is securely transmitted to the operating system or network authentication server.  
3. **System verifies credentials** – Password is checked against stored hashes or authentication protocols (e.g., Active Directory, LDAP).  
4. **Authentication result returned** – If credentials match, access is granted; otherwise, the login fails.  
5. **Session is created** – The system generates a session token or context so the user can interact with resources without re-entering credentials.  
6. **Access permissions applied** – User is given access to files, applications, and system resources according to their account privileges.  
7. **Optional multi-factor authentication (MFA)** – If enabled, the system prompts for a secondary factor, such as a code from a mobile app or security key.  

## Operational/Security Considerations
- **Password strength** is critical; weak passwords make accounts vulnerable.  
- **Account lockout policies** help prevent brute-force attacks.  
- **Encrypted transmission** (e.g., TLS) prevents credentials from being intercepted.  
- **Session expiration** ensures users are automatically logged out after inactivity.  

## How This Breaks or Gets Attacked
- **Incorrect password or misconfigured account** prevents login.  
- **Expired or revoked credentials** can block access.  
- **Keyloggers or phishing attacks** can steal user credentials.  
- **Session hijacking** could allow attackers to impersonate logged-in users.  
