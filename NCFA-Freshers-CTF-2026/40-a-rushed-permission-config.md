# 40 — A Rushed Permission Config

**Category:** Linux  |  **Difficulty:** Easy

**Flag:** `LUNA{SUDO_SU}`

## How I found the flag

- Entrypoint ran setfacl -m u:inspecto:rw /etc/sudoers.
- So our user can write /etc/sudoers.
- Appended a NOPASSWD rule, then sudo cat /root/flag.txt.
- NOTE: flag format is LUNA{...} for this one.

