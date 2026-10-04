# 36 — Operation Phantom OSINT 4 - Commit and Forget

**Category:** OSINT  |  **Difficulty:** Hard

**Flag:** `NCFA{d3l3t3d_but_n0t_g0ne}`

## How I found the flag

- Live credential in a deleted .env.backup: git show 1b1cb36:.env.backup.
- A decoy NCFA{r0tat3d_and_r3v0k3d} (old config.ini) is REVOKED.
- Commit 027e13a says the decoy is dead -> read commit messages first.
- Real flag = the live one from .env.backup.

