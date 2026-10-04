# 09 — Plain Sight

**Category:** Reversing  |  **Difficulty:** Easy

**Flag:** `NCFA{rodata_remembers_everything}`

## How I found the flag

- Binary carries decoys: ACME{...}, base64 traps, hunter2.
- Extract Strings alone misleads you.
- The real flag sits plainly in the .rodata section.
- Picked the NCFA{...} string out of the noise.

