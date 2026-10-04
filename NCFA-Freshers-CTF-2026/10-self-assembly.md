# 10 — Self Assembly

**Category:** Reversing  |  **Difficulty:** Medium

**Flag:** `NCFA{never_trust_the_output}`

## How I found the flag

- Python builds the flag two ways.
- Default run prints decoy summary() = NCFA{almost_but_not_quite}.
- Real flag comes from build() = A XOR B.
- B is a 4-byte repeating key -> XOR -> real flag.

