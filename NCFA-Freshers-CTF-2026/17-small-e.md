# 17 — Small e

**Category:** Crypto  |  **Difficulty:** Medium

**Flag:** `NCFA{integ3r_r00ts_betray_y0u}`

## How I found the flag

- RSA with e=3 and no padding; message much smaller than n.
- No modular reduction happened (m^3 < n).
- Took the integer cube root of c -> plaintext -> flag.

