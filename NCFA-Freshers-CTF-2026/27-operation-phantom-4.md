# 27 — Operation Phantom 4

**Category:** Forensics  |  **Difficulty:** Easy

**Flag:** `NCFA{l0ok_b&yohd_the_p1ctur&}`

## How I found the flag

- JPEG with a steghide-embedded note.txt (empty passphrase).
- No local steghide -> used the futureboy.us online decoder via curl.
- Extracted the note -> flag.

