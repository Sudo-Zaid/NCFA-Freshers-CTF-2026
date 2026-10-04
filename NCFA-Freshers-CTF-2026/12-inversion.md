# 12 — Inversion

**Category:** Reversing  |  **Difficulty:** Hard

**Flag:** `NCFA{inverting_is_reversing}`

## How I found the flag

- Static ELF checks ((input[i]^key[i&3])+i)&0xff == exp[i].
- 4-byte key @ 0x4010, 24-byte expected @ 0x4020.
- Inverted the transform -> password Inv3rt_Th3_Transf0rm_Now.
- POSTed the password to the launched web form; server returned the flag (password != flag).

