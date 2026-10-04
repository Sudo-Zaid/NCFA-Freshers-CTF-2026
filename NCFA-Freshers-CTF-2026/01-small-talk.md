# 01 — Small Talk

**Category:** Pwn  |  **Difficulty:** Easy

**Flag:** `NCFA{percent_p_walks_the_stack}`

## How I found the flag

- Source feeds user input straight into printf(input) (no format string).
- Sent a chain of %p through the web form to dump the stack.
- The secret char[64] sits a few args in; its raw bytes show from arg offset ~22.
- Decoded the little-endian hex of those slots into the flag.

