# Troubleshooting

Adapted from TROUBLESHOOTING.md in the AI Memory Vault by Jared Rhodenizer (github.com/jaredrhod/ai-memory-vault), CC BY-SA 4.0.

Written for people and for AI assistants. If you're an AI helping someone with this vault: read this file, then work from their actual files and folders, never from guesses.

## Where are my notes, physically?

Open `My Business Vault/VAULT-INDEX.md`: its "Vault location" section has the full path. The notes are the `My Business Vault` folder inside this kit folder. Obsidian also knows: its vault switcher lists every vault with its path.

## Obsidian opened to a welcome screen instead of my notes

Obsidian only opens folders it has been shown once. On the welcome screen choose **Open folder as vault** and pick the `My Business Vault` folder. It remembers from then on.

## How do I back up my notes?

The notes live on one computer. Pick any one of these free options:

- **Windows:** File History (Settings, then search "File History", turn it on with an external drive, and add the kit folder to its list once).
- **Mac:** Time Machine covers your home folder automatically if the kit is there.
- **Copy:** once a week, copy the whole kit folder to a USB drive.

Don't put the vault in two sync services at once (for example OneDrive and Obsidian Sync). Two sync tools editing the same files make conflicted copies.

## My notes are in OneDrive or iCloud

That works and gives you a free backup. One click keeps it fast: right-click the kit folder and choose "Always keep on this device" (Windows) or "Keep Downloaded" (Mac), so the cloud doesn't swap your notes for online-only placeholders.

## The AI says it can't find my notes

The vault path is written in two places: `AGENTS.md` in the kit folder and the "Vault location" section of `VAULT-INDEX.md`. If you moved the folder, tell the AI the new path and have it update both (and the MEMORY.md pointer if you set one up). Also make sure your assistant has the kit folder open, not somewhere else (see "Where the rules load from" below for your path).

## The AI isn't following the rules or doesn't know my business

Check that the rules file can load on your path (see "Where the rules load from" below). In a long conversation, say "re-read your vault index". If an answer is wrong, correct it and ask it to fix the note the answer came from.

## Where the rules load from

### On Claude Code

`AGENTS.md` loads from the folder Claude Code was opened in. If it ignores the rules, reopen Claude Code in the kit folder.

### On Codex

`AGENTS.md` loads from the folder opened in the Codex app as a local folder. Codex on the chatgpt.com web page cannot see a folder on your computer. If it ignores the rules, reopen the kit folder in the Codex app and say "Please read AGENTS.md and VAULT-INDEX.md now."

### On the Claude desktop chat

The chat has no folder of its own. The rules load only through the one-line preference you saved (Settings, then Profile, then personal preferences) and the Filesystem extension pointed at the kit folder. If it ignores the rules, say "Please read AGENTS.md and VAULT-INDEX.md now." Then check that the preference is saved and that the extension's allowed folders include the kit folder.

## The AI asks for permission a lot

That's the safe setting working. Don't switch to "bypass permissions" or any mode that never asks; it would let the AI send, post or delete without you.
