# 31 — Operation Phantom 5 - The Break-In

**Category:** Forensics  |  **Difficulty:** Easy

**Flag:** `NCFA{admin}`

## How I found the flag

- Security log of logins.
- admin failed 7 times from 192.168.9.66 then suddenly SUCCESS.
- Right after: settings changed + audit_log deleted.
- (sam's single fail was an honest typo.) Compromised account = admin.

