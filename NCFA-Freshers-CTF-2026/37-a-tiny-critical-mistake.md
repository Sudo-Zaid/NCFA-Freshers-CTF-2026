# 37 — A Tiny Critical Mistake

**Category:** Linux  |  **Difficulty:** Easy

**Flag:** `NCFA{CP_GTFOBINS}`

## How I found the flag

- SSH jack/jack; /usr/bin/cp is SUID root (GTFOBins).
- Built a new /etc/passwd with an extra uid-0 user r (openssl-generated hash).
- Used SUID cp to overwrite /etc/passwd.
- su r -> root -> /root/flag.txt.

