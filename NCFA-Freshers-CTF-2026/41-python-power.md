# 41 — Python Power

**Category:** Linux  |  **Difficulty:** Easy

**Flag:** `NCFA{pyth0n_r3plac3m3nt}`

## How I found the flag

- SSH ncfa/ncfa; sudo -l (pw ncfa) allows (root) /usr/bin/python3 /home/ncfa/coolpython.py.
- That script file is writable by ncfa.
- Overwrote it with a payload that reads /root/flag.txt.
- Ran it via sudo -> executes as root -> flag.

