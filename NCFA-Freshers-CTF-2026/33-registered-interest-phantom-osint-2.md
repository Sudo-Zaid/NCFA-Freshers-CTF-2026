# 33 — Registered Interest - Phantom OSINT 2

**Category:** OSINT  |  **Difficulty:** Medium

**Flag:** `NCFA{phantomrelay}`

## How I found the flag

- Had a crt.sh certificate-transparency export and a 34-host brute scan set.
- Set-diff'd them.
- One extra host only in CT logs: phantomrelay.vantabyte-logistics.co.uk.
- Flag = the subdomain label, phantomrelay.

