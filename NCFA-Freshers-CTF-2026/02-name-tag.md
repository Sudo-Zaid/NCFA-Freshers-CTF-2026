# 02 — Name Tag

**Category:** Pwn  |  **Difficulty:** Easy

**Flag:** `NCFA{one_too_many_letters}`

## How I found the flag

- scanf("%s", name) writes into a 32-byte buffer with no length limit.
- int staff sits right after name[] in the struct.
- Sent 40 A's so the overflow fills staff with non-zero.
- if (staff) is now true and the flag prints.

