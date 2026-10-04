# 32 — Loud Whispers

**Category:** Forensics  |  **Difficulty:** Medium

**Flag:** `NCFA{tunnelled_through_lookups}`

## How I found the flag

- Capture full of DNS queries like <idx>.<hexchunk>.cdn-metrics.invalid.
- Ordered chunks by idx 0-9, concatenated the hex, decoded.
- Result: host=FIN-LT-051;user=r.hale;note=NCFA{...};end (parsed with scapy DNSQR).

