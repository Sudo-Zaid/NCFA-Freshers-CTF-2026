# 22 — Cut Short

**Category:** Forensics  |  **Difficulty:** Hard

**Flag:** `NCFA{unwiped_and_unshrunk}`

## How I found the flag

- FAT12 floppy image with a deleted PLAN.PNG (0xE5 marker).
- Carved it from contiguous clusters.
- IHDR said height 430 but IDAT held 600 rows.
- Patched height + fixed CRC -> bottom of the image reveals the door code.

