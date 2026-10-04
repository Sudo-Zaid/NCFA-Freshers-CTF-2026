# 08 — Wrapped Up

**Category:** Reversing  |  **Difficulty:** Easy

**Flag:** `NCFA{peel_the_onion}`

## How I found the flag

- A Python script wraps a payload a few layers deep.
- Chain: base64 -> rot13 -> base64 -> source code.
- Decoded it statically (did not exec).
- Inner source holds secret = 'NCFA{peel_the_onion}'.

