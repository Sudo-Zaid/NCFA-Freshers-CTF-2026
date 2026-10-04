# 04 — Trapdoor

**Category:** Pwn  |  **Difficulty:** Medium

**Flag:** `NCFA{go_where_it_never_calls}`

## How I found the flag

- Non-PIE x64 with a hidden prize() @ 0x401236 that reads flag.txt.
- vuln buffer at [rbp-0x40], reads 0x100 bytes -> overflow offset 72.
- Payload = 72*'A' + p64(0x401236).
- Sent via the HTTP form in hex mode (payload=...&mode=hex).

