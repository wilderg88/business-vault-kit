<!-- Based on the AI Memory Vault by Jared Rhodenizer (github.com/jaredrhod/ai-memory-vault), CC BY-SA 4.0.

This file is NOT a vault note. It is the pointer for Claude Code's own memory file, so there is only one memory: the vault.

Where it goes: Claude Code keeps a memory folder for each folder you open it in, under  ~/.claude/projects/<folder name with dashes>/memory/MEMORY.md  (on Windows  C:\Users\<you>\.claude\projects\...). The folder that matters is the one for THIS kit folder (where AGENTS.md lives), not any other. Easiest way: open Claude in this kit folder and ask "where is your MEMORY.md file for this folder?"

SETUP.md does this step for you: it copies anything already in that memory file into the vault first (copy, never move or delete), then, with your yes, replaces the file's contents with the text below, with the real vault path filled in. If you use the Claude desktop app without Claude Code, skip this file. -->

There is no separate memory layer here. The single source of truth is the Obsidian vault, located at:

    [FILL IN: full vault path, the same one in VAULT-INDEX.md "Vault location"]

Read the vault from there at the start of every session. Sources of truth, in load order:
- AGENTS.md (in the kit folder, NOT in the vault): who the assistant is, the startup steps and the rules that can't lapse.
- VAULT-INDEX.md (at the vault root): the owner's profile, the full rules and the map.
- Everything else lives in its own note in the vault.

To remember something, write it to its place in the vault, never here.
