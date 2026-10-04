# 29 — Hidden In Plain Sight

**Category:** Forensics  |  **Difficulty:** Medium

**Flag:** `NCFA{Hidden_In_Zero_Width_Sight}`

## How I found the flag

- Text hides zero-width chars (U+200B = 0, U+200C = 1).
- Extracted the bit string.
- XOR'd it with the visible sentence 'You really don't want to know!' -> flag.

