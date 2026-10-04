# 21 — Signature Required

**Category:** Forensics  |  **Difficulty:** Easy

**Flag:** `NCFA{picture_resurrected}`

## How I found the flag

- A .png that no viewer opens.
- First 8 bytes (PNG signature) were zeroed.
- Restored 89 50 4E 47 0D 0A 1A 0A.
- Image opens and shows the flag.

