# 03 — Overdrawn

**Category:** Pwn  |  **Difficulty:** Easy

**Flag:** `NCFA{minus_makes_you_rich}`

## How I found the flag

- Bank starts at 50 credits; souvenir costs 1000.
- Withdraw does balance -= amt with no sign check.
- Withdrew -1000 so balance became 1050.
- Payload: 2 (withdraw), -1000, then 3 (buy) -> flag.

