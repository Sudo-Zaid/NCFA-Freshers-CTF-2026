# 06 — Switchboard

**Category:** Pwn  |  **Difficulty:** Medium

**Flag:** `NCFA{bend_the_call_elsewhere}`

## How I found the flag

- A 64-byte note buffer sits next to a function pointer.
- Overflowing the note overwrites that pointer.
- Redirected it to prize (0x401236).
- Program calls the pointer -> prize prints the flag.

