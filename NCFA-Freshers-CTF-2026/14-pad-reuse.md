# 14 — Pad Reuse

**Category:** Crypto  |  **Difficulty:** Hard

**Flag:** `NCFA{key_reuse_breaks_it_all}`

## How I found the flag

- Six ciphertexts XOR'd with the SAME keystream.
- Dragged the crib 'The quick brown fox' to lock part of the key.
- msg1/msg4 cribs extended the keystream across the length.
- Recovered msg3 = the flag.

