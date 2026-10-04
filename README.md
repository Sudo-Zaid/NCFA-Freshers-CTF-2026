# NCFA Freshers CTF 2026 — Writeups

Solved challenges from the **NCFA Freshers CTF** (hosted on the Biterra platform, flag format `NCFA{...}`).
Each file is a short writeup: challenge info, the flag, and how I found it.

## 🏆 Result

> ### 🥇 1st Place — Individual (competed **solo**) — **4125 points**
> Also **3rd Place Overall** on the team board as a **one-person team** (*wargaye* 🐐) — out-scoring full multi-member squads.

| Board | Placement | Score |
|-------|-----------|------:|
| **Individual** | 🥇 **1st** (solo) | **4125** |
| Overall (teams) | 🥉 3rd — one-person team | 4125 |

**Total solved: 41** across 7 categories — Pwn, Reversing, Crypto, Web, Forensics, OSINT and Linux.

| # | Challenge | Category | Difficulty | Key technique |
|---|-----------|----------|------------|---------------|
| 01 | [Small Talk](01-small-talk.md) | Pwn | Easy | Format-string stack leak |
| 02 | [Name Tag](02-name-tag.md) | Pwn | Easy | Buffer overflow into adjacent int |
| 03 | [Overdrawn](03-overdrawn.md) | Pwn | Easy | Signed integer, no bounds check |
| 04 | [Trapdoor](04-trapdoor.md) | Pwn | Medium | ret2win (non-PIE) |
| 05 | [Borrowed Tools](05-borrowed-tools.md) | Pwn | Hard | ret2libc with printf leak |
| 06 | [Switchboard](06-switchboard.md) | Pwn | Medium | Overflow into function pointer |
| 07 | [Password Please](07-password-please.md) | Reversing | Easy | Password built at runtime (strcat) |
| 08 | [Wrapped Up](08-wrapped-up.md) | Reversing | Easy | Nested encoding |
| 09 | [Plain Sight](09-plain-sight.md) | Reversing | Easy | Flag plain in .rodata |
| 10 | [Self Assembly](10-self-assembly.md) | Reversing | Medium | Decoy function vs real build |
| 11 | [Simple C Strings](11-simple-c-strings.md) | Reversing | Easy | Hardcoded string |
| 12 | [Inversion](12-inversion.md) | Reversing | Hard | Invert a byte transform |
| 13 | [Caesar Salad](13-caesar-salad.md) | Crypto | Easy | Per-word Caesar |
| 14 | [Pad Reuse](14-pad-reuse.md) | Crypto | Hard | Many-time pad |
| 15 | [Rhythm Section](15-rhythm-section.md) | Crypto | Medium | Vigenere break |
| 16 | [Single Byte](16-single-byte.md) | Crypto | Easy | Single-byte XOR |
| 17 | [Small e](17-small-e.md) | Crypto | Medium | RSA e=3 cube root |
| 18 | [Operation Phantom 6 - The Locked Confession](18-operation-phantom-6-the-locked-confession.md) | Crypto | Easy | Caesar shift |
| 19 | [Mind the Gap](19-mind-the-gap.md) | Crypto | Easy | Whitespace stego (uncertain) |
| 20 | [Northbridge SQL Injection](20-northbridge-sql-injection.md) | Web | Easy | SQLi auth bypass |
| 21 | [Signature Required](21-signature-required.md) | Forensics | Easy | Fix PNG magic bytes |
| 22 | [Cut Short](22-cut-short.md) | Forensics | Hard | FAT12 carve + PNG height patch |
| 23 | [Over the Wire](23-over-the-wire.md) | Forensics | Easy | HTTP pcap carve |
| 24 | [Uninvited Commit](24-uninvited-commit.md) | Forensics | Easy | Git deleted-file recovery |
| 25 | [Operation Phantom 1](25-operation-phantom-1.md) | Forensics | Easy | EXIF GPS |
| 26 | [Operation Phantom 3](26-operation-phantom-3.md) | Forensics | Easy | Hidden dotfile |
| 27 | [Operation Phantom 4](27-operation-phantom-4.md) | Forensics | Easy | steghide (empty pass) |
| 28 | [Quiet Pixels](28-quiet-pixels.md) | Forensics | Medium | LSB stego |
| 29 | [Hidden In Plain Sight](29-hidden-in-plain-sight.md) | Forensics | Medium | Zero-width stego |
| 30 | [Signal Intercept](30-signal-intercept.md) | Forensics | Easy | DTMF decode |
| 31 | [Operation Phantom 5 - The Break-In](31-operation-phantom-5-the-break-in.md) | Forensics | Easy | Auth-log brute-force spot |
| 32 | [Loud Whispers](32-loud-whispers.md) | Forensics | Medium | DNS exfil |
| 33 | [Registered Interest - Phantom OSINT 2](33-registered-interest-phantom-osint-2.md) | OSINT | Medium | CT-log vs scan diff |
| 34 | [Wayback When - Phantom OSINT 3](34-wayback-when-phantom-osint-3.md) | OSINT | Medium | Wayback Machine |
| 35 | [Operation Phantom OSINT 1 - Handle With Care](35-operation-phantom-osint-1-handle-with-care.md) | OSINT | Easy | Username pivot |
| 36 | [Operation Phantom OSINT 4 - Commit and Forget](36-operation-phantom-osint-4-commit-and-forget.md) | OSINT | Hard | Git deleted secret + decoy |
| 37 | [A Tiny Critical Mistake](37-a-tiny-critical-mistake.md) | Linux | Easy | SUID cp -> /etc/passwd |
| 38 | [CowTooStrong](38-cowtoostrong.md) | Linux | Easy | sudo cowthink GTFOBins |
| 39 | [A Long History Reveals All](39-a-long-history-reveals-all.md) | Linux | Medium | bash_history token -> OpenBao |
| 40 | [A Rushed Permission Config](40-a-rushed-permission-config.md) | Linux | Easy | setfacl-writable sudoers |
| 41 | [Python Power](41-python-power.md) | Linux | Easy | sudo on a writable script |

## Categories

- **Pwn** — 6
- **Reversing** — 6
- **Crypto** — 7
- **Web** — 1
- **Forensics** — 12
- **OSINT** — 4
- **Linux** — 5

## Notes

- Two Linux challenges (*A Long History Reveals All*, *A Rushed Permission Config*) use the `LUNA{...}` flag format, not `NCFA{...}`.
- *Mind the Gap* flag is marked uncertain (decoded from hand-typed text) — re-decode from the exact source to confirm.

---

See [COPYRIGHT.md](COPYRIGHT.md).
