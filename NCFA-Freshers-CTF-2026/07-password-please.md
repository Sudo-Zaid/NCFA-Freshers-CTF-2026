# 07 — Password Please

**Category:** Reversing  |  **Difficulty:** Easy

**Flag:** `NCFA{glued_at_runtime}`

## How I found the flag

- strings is useless: the password is assembled in build_password().
- Seven rodata pieces strcat'd: Fa+l7o+ns_+Fly+_At+_Da+wn.
- = Fal7ons_Fly_At_Dawn.
- POSTed that password to the challenge web form -> flag.

