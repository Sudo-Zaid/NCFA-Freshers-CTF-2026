# 20 — Northbridge SQL Injection

**Category:** Web  |  **Difficulty:** Easy

**Flag:** `NCFA{LOGIN_BYPASSED}`

## How I found the flag

- Admin login form POSTs to login.php.
- The username field is injectable.
- Sent admin' -- - to comment out the password check.
- Logged in -> dashboard shows the flag.

