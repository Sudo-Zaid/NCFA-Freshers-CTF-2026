# 39 — A Long History Reveals All

**Category:** Linux  |  **Difficulty:** Medium

**Flag:** `LUNA{Those_who_cannot_remember_the_past_are_condemned_to_repeat_it}`

## How I found the flag

- Checked .bash_history.
- Found export BAO_TOKEN=arootkeyforopenbao.
- Used OpenBao: bao kv get secret/root-flag.
- NOTE: this challenge's flag format is LUNA{...}, not NCFA - submit the literal LUNA flag.

