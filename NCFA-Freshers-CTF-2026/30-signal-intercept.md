# 30 — Signal Intercept

**Category:** Forensics  |  **Difficulty:** Easy

**Flag:** `NCFA{GOTTHECODE}`

## How I found the flag

- Audio of phone key tones.
- Decoded DTMF with a Goertzel filter -> PIN 08753.
- Submitted the PIN to /api/verify -> flag.

