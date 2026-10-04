# 05 — Borrowed Tools

**Category:** Pwn  |  **Difficulty:** Hard

**Flag:** `NCFA{one_leak_is_all_it_takes}`

## How I found the flag

- Non-PIE + NX; a printf leak reveals a libc address (glibc 2.39).
- Web form caps input at 256 bytes and gives no stdin.
- Wrote a short command into .bss using a libc mov [rsi],rdi gadget.
- Then called system(bss) for command execution -> flag.

