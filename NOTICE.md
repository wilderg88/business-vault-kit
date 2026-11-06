# Notice and credit

This kit is an adapted version of the **AI Memory Vault** by **Jared Rhodenizer** (@jaredrhod):

https://github.com/jaredrhod/ai-memory-vault

Source version used: commit 659bba9c8b351c937dd393b3042801d1ff1b502c, read 2026-10-31.

Original work Copyright (c) 2026 Jared Rhodenizer, licensed under Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0). This adapted version is licensed under the same license, CC BY-SA 4.0 (full text in LICENSE, and at https://creativecommons.org/licenses/by-sa/4.0/). If you share or adapt this kit, keep this credit and use the same license. No warranty is given; see the license.

The way the system works is Jared's: one memory (the vault), a short boot file outside the vault, startup reads, saving the same turn, Job notes, folder indexes kept current, daily notes from a template, and a living profile.

## What was changed

| Jared's file | This kit | What changed |
|---|---|---|
| upstream assistant start-up template | AGENTS.md | Same structure, startup steps and core rules. The shipped "Jarvis" personality (profane, for a developer) is replaced by a warm, plain business assistant (default name Penny) since the drafts go to customers. "Double-confirm before any source-code edit" became "Nothing leaves without my yes" (no sending, posting, buying or account changes without a yes), because this assistant reaches inboxes, not code. Added a permission-settings warning: never use bypass modes. Vault path points at the My Business Vault folder next to the boot file. Plain words throughout. |
| templates/VAULT-INDEX.md | My Business Vault/VAULT-INDEX.md | Same two jobs (profile and map) and the same vault rules, reworded in plain words. Profile sections fit a business (My Business, Key People). Vault Structure lists the eight business folders. Added a "Settled answers" pointer to Settled-Facts and the FAQ. One project slug (`business`). Optional personal sections cut to three. Writing rules add short, warm customer replies. |
| templates/MEMORY.md | MEMORY.md | Same pointer text; instructions in plain words and point at this kit folder. |
| templates/DAILY-NOTE.md | My Business Vault/01 - Daily Notes/Daily Note Template.md | Same sections. Project set to `business`; a comment that decisions also go to their own note; em-dashes removed. |
| ai-memory-vault.md | SETUP.md | Shortened. Jared's build file interviews a person and creates the folders; here the business folders ship ready, so setup keeps his order (check access and Obsidian, welcome, interview, preview and confirm, build, one memory, verify and onboard) but only fills in blanks. Kept: install Obsidian with the owner's OK, Jared's full memory migration (find every memory file, copy never move, consolidate, frozen archive read back, then a pointer only on a yes, never delete), backup sentence. Added: permission-mode check, a 5-minute "teach it your business" step. Left out: the full folder build, hand-editing Obsidian's registry file, the Desktop launcher, and the offers for Jared's other tools (voice, face, hands, marketing files), to keep setup safe and short for a non-technical owner. Jared's original is at the link above. |
| TROUBLESHOOTING.md | TROUBLESHOOTING.md | Same topics (where are my notes, welcome screen, backups, cloud sync, AI can't find the vault), rewritten for the kit's folder layout; added two entries (AI not following rules, permission prompts). |
| README.md | README.md | New README for a small-business owner; credits Jared at the top. |
| LICENSE | LICENSE | Unchanged (CC BY-SA 4.0). |
| (none) | My Business Vault folders 00 to 07 with index notes, Settled-Facts.md, Active Priorities.md, FAQ.md, Jobs.md, Job template.md, two example Jobs | New, built from the formats in Jared's build file (folder index, Active Priorities, Job note and worked example). Example data is made up. |
| (none) | My Business Vault/.obsidian/app.json | Turns on "Automatically update internal links", as Jared's build file does. |
| .gitignore | (left out) | Not needed for a folder kit. |
