# My Business Vault: a memory for your AI assistant

**Built on the AI Memory Vault by Jared Rhodenizer:** https://github.com/jaredrhod/ai-memory-vault (CC BY-SA 4.0). The way it works is his. Changes are listed in NOTICE.md.

## What it is

A folder of plain notes that becomes your AI assistant's memory. Every time you talk to it, it reads these notes first, so it already knows your business: your hours, prices, policies, events, vendors, and the answers you give to the questions people ask you over and over. When you tell it something new, it writes it down the same day. You never explain the same thing twice.

## Who it's for

Small-business owners who aren't technical. If you can open a folder and type a sentence, you can set this up.

## What you need

- A computer (Windows or Mac).
- **The vault itself is free.** Pick one of these ways to run it:
  - **Claude Pro** (about $20 a month, claude.com/pricing): the smoothest path. It opens this folder directly and follows the kit's rules on its own.
  - **ChatGPT Plus** (chatgpt.com/pricing) with Codex: also opens this folder directly. Both pages checked 2026-11-02.
  - **Free: Codex on ChatGPT's free plan.** Codex access on the free plan is limited, so long sessions may stop until the limit resets.
  - **Free: the Claude desktop chat with its filesystem extension**, which lets Claude read and write this folder. You set it up yourself (see SETUP.md). Claude Free usage is limited, and this path has not been tested on a real Free account.
- **Obsidian**, a free app for seeing your notes (obsidian.md).

## INSTALL GUIDE

Your AI follows the full INSTALL GUIDE in `SETUP.md` with you, one step at a time, doing what it can and guiding the rest.

1. Get the business kit at https://sites.wilderautomates.com/mockups/business-vault/. Unzip into Documents with a simple folder name.
2. Install the Codex app from https://openai.com/codex, sign in with your ChatGPT account, and open the kit folder locally, not on chatgpt.com. Or use Claude Code in Claude desktop, or desktop chat with the Filesystem extension set to ask each time. The agent guides sign-in and opening the folder; it cannot install itself.
3. Back up the whole kit folder before any write.
4. Keep default approval. Never choose full access or bypass permissions.
5. Say yes if you want the agent to install Obsidian with winget on Windows or brew on Mac. Otherwise use https://obsidian.md. Choose **Open folder as vault** and select the inner `My Business Vault` folder.
6. Paste: `Read SETUP.md and set me up.` Then answer the interview one topic at a time.
7. Ask the agent to list what is installed and working and help with anything left. See `TROUBLESHOOTING.md` if needed.

## Your first hour

1. **Install the apps.**
   - Your AI tool: Claude desktop app (claude.com/download) or the Codex app (from openai.com/codex), signed in with your ChatGPT account.
   - Obsidian: download it free from obsidian.md and install it. (Or skip this; on Claude Code or Codex, setup in step 3 offers to install it for you. On the chat path, download it from obsidian.md.)
2. **Put this kit somewhere you'll find it**, like your Documents folder. Keep the folder name simple.
3. **Open the kit folder in your AI tool.** Pick one path (SETUP.md has the full steps for each):
   - **Claude Code** (paid Claude plan): in the Claude desktop app choose **Claude Code**, then pick this kit folder. It reads `AGENTS.md` on its own (version 2.1.277 or newer).
   - **Codex**: in the Codex app, sign in with your ChatGPT account and open this kit folder as a local folder. It reads `AGENTS.md`. Codex on the chatgpt.com web page cannot see a folder on your computer, so use the app.
   - **Claude desktop chat** (works on the free plan): install the filesystem extension, point it at this kit folder, save the one-line preference naming `AGENTS.md` and `VAULT-INDEX.md`, and keep tool approval on ask each time.

   Before the first note is written, make a backup copy of the kit folder. Then paste this one sentence:

   > Read SETUP.md and set me up.

   It checks everything, asks you some short questions about you and your business, and fills in your notes. About ten minutes.
4. **Open your notes in Obsidian.** Choose **Open folder as vault** and pick the `My Business Vault` folder inside the kit. That's your assistant's memory; everything it learns shows up here.
5. **Teach it your business (5 minutes).** At the end of setup it asks for your hours, your main prices, your policies, and the 10 questions you get asked most, with your answers. From then on it drafts replies from those answers.

After that, just talk to it. Open your AI tool in the kit folder whenever you want your assistant.

## Use it from your phone (optional, later)

Once the local kit works, you can keep a copy on GitHub so your AI can read and save notes from your phone with the computer off. Needs a paid Claude plan (Claude Code in the Claude phone app). Tested once with Claude Code on a Pro-or-higher plan; other AI apps are not confirmed.

1. On GitHub, open this repo and click **Use this template**, then **Create a new repository**. Set it to **Private**. Never public.
2. Install the Claude GitHub App on your GitHub account and choose **Only select repositories**, then pick only that one repo.
3. In the Claude phone app, open the **Code** tab and start a session on that repo.
4. Start every session with this one line: `Read AGENTS.md first. Save only by creating a new file in vault/inbox/, commit it to the default branch, and give me the commit link.`
5. Check on GitHub that the new note is on the main branch. Notes saved from the phone land in `vault/inbox/`; your AI files them into the right folders the next time you work on your computer.

Keep real customer details out of the cloud copy unless the customer agreed in writing. If a note can't be saved, the AI returns it in the chat marked MANUAL SAVE REQUIRED; paste it into the GitHub phone editor.

## What's inside

- `AGENTS.md`: who your assistant is and the rules it always follows. Claude Code and Codex both read it.
- `SETUP.md`: the setup steps the assistant follows with you.
- `My Business Vault/`: your notes. Inbox, Daily Notes, Customers and FAQ, Events and Calendar, Vendors and Partners, Marketing and Content, Archive, Resources and Jobs, plus Settled-Facts (your official answers) and Active Priorities (your to-do list).
- `TROUBLESHOOTING.md`: fixes for common problems.

## Stay safe

- **Never paste passwords, card numbers or codes into a chat.** You type your own passwords where the app asks.
- **Keep the safe permission setting.** Use the mode that asks before risky actions (Auto in Claude Code, the default approval mode in Codex, ask each time in the Claude desktop chat). Don't turn on "bypass permissions" or any mode that lets the AI act without asking.
- **Nothing gets sent without you.** The assistant drafts replies and posts; you approve them.
- **Keep a backup** of the kit folder (see TROUBLESHOOTING.md). The notes live only on your computer.

## Credit and license

The AI Memory Vault is by Jared Rhodenizer, https://github.com/jaredrhod/ai-memory-vault. This kit is shared under the same license, CC BY-SA 4.0 (see LICENSE and NOTICE.md). You can use and change it, including in your business. If you share a changed version, credit Jared and use the same license.
