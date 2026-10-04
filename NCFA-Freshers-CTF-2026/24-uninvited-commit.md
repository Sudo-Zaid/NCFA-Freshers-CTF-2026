# 24 — Uninvited Commit

**Category:** Forensics  |  **Difficulty:** Easy

**Flag:** `NCFA{rewound_but_recorded}`

## How I found the flag

- Git repo with a deleted scripts/build-helper.sh (malicious postinstall hook).
- Recovered it via git show 7f1714b:scripts/build-helper.sh.
- The operation tag is in a comment; payload was a base64 curl|sh.

