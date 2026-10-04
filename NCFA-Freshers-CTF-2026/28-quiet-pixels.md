# 28 — Quiet Pixels

**Category:** Forensics  |  **Difficulty:** Medium

**Flag:** `NCFA{quiet_colours_confess}`

## How I found the flag

- Image with data hidden in the least-significant bits.
- Read LSBs RGB-interleaved, MSB-first.
- Reassembled bytes -> flag.

