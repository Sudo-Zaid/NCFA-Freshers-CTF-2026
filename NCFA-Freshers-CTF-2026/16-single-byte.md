# 16 — Single Byte

**Category:** Crypto  |  **Difficulty:** Easy

**Flag:** `NCFA{single_byte_is_no_lock}`

## How I found the flag

- Single-byte XOR ciphertext.
- Key = first byte ^ 'N' = 0x5A.
- XOR'd the whole buffer -> flag.

