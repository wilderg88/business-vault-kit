---
status: active
project: meta
type: index
---
# VAULT INDEX

Read this file at the start of every conversation. It has two jobs: **who I am and how my business works** (the profile) and **the map of this vault** (the folders, the indexes and the rules for keeping them). The assistant's own identity lives in AGENTS.md, outside this vault.

(Based on the AI Memory Vault by Jared Rhodenizer, github.com/jaredrhod/ai-memory-vault, CC BY-SA 4.0.)

(**AI:** if any [FILL IN: ...] markers remain, this vault isn't set up yet. Offer to interview the owner, one topic at a time, in plain words. Explain in one line why each section helps, make clear the personal sections are optional, and never press. Write their answers in the first person, as if they wrote it, delete sections they skip, and delete this block and every other note in brackets when done.)

---

## Vault location

This vault lives at `[FILL IN: full path to the My Business Vault folder]`. This line is the single source of truth for the path. The same path is written in AGENTS.md and in Claude's MEMORY.md pointer; if the vault moves, update all of them in the same pass. If you use the Claude desktop app or another AI, point it at this folder and tell it "my vault is here".

---

## Who I Am

[FILL IN: your name, your business, what you sell or do, where you're based if you want to share it. First person, a few lines.]

## My Business

[FILL IN: business name, what it does, who the customers are, how they find you (Instagram, website, word of mouth), and the tools you already use (email, Instagram, booking or payment apps).]
- **Status:** [FILL IN: e.g. open and growing]

## Key People

[FILL IN: one line per important person: partners, staff, family who help, key vendors or venues.]
- **[[Name]]**: [FILL IN: who they are to the business]

## Vault Structure

```
00 - Inbox                ← drop anything here, sort later
01 - Daily Notes          ← what got done each day, one file per day
02 - Customers and FAQ    ← customers, the questions they ask and the answers I give
03 - Events and Calendar  ← events, dates, venues and schedules
04 - Vendors and Partners ← vendors, suppliers, venues and partners
05 - Marketing and Content← posts, videos, ads, flyers, email ideas
06 - Archive              ← finished or old notes
07 - Resources and Jobs   ← reference material and the Job notes (how to do recurring tasks)
Settled-Facts.md          ← my official answers: hours, prices, policies
Active Priorities.md      ← the one list of everything open
```

## What's Active Right Now

All open work lives in one note: [[Active Priorities]]. Check it at the start of every conversation, and check an item's real state before acting on it (it may already be done).

## Settled answers

My official answers (hours, prices, policies, how things work) live in [[Settled-Facts]]. Before answering a customer or vendor question, check there and in [[Customers and FAQ]]. If the answer isn't there, ask me; never invent one.

(Optional sections. Skip or delete any of them; the system loses nothing.)

## How I Work
[FILL IN: bullets, first person: how you like to run things, what you care about most.]

## Daily Routine
[FILL IN: bullets: when you work, busy days, when markets or events happen.]

## What I Want
[FILL IN: what you're building toward this year. The assistant can only weigh choices the way you would if it knows this.]

## How I Like to Work with the AI

- **Plain words, no jargon, be direct.** Be honest and upfront.
- **Do it right the first time.** Don't park a known problem for later.
- **Be a partner, not a yes-man.** Tell me when you think I'm wrong, give the reason, then let me decide.
- **Draft for me.** When something needs writing (a reply, a post, an email), offer a draft that sounds like me. I decide what goes out.
- **Restating isn't approving.** If I think out loud about an option, that's not a yes. Save it as final only when I clearly say so.
- **I decide on access.** Never ask for more access or connect new apps on your own. More access comes from me.

---

## How My Memory Works (for the AI)

This vault is your memory. It is outside your head and has no size limit. Don't try to hold all of it. Hold what the current task needs and trust that everything else is one search away: start at this index, follow the folder indexes and links, or search. Knowing a note exists is as good as holding it.

---

## Vault Rules for AI

(These rules are for the assistant. You never need to edit the technical bits yourself: the block at the top of each note and the [[double-bracket]] links between notes are kept by the assistant.)

### Frontmatter and links

Every note has YAML frontmatter. When you create a note, include it; when you edit a note missing it, add it. Don't ask me what the values should be; work them out.

```yaml
---
status: active
project: business
type: reference
---
```

When creating or editing a note, add `[[wikilinks]]` to people in Key People, named businesses, venues, platforms, and any note this one depends on. Don't link generic words, the same target twice, or the note's own title.

**status:** `active` | `completed` | `parked` | `idea` | `archived`
**project:** `business` | `personal` | `meta` (the Inbox: work it out from the content)
**type:** `index` (folder index) | `reference` (looked-up facts) | `guide` (how-to, Job notes) | `plan` (Active Priorities) | `log` (daily notes)

### Note format

Simple and readable. No random emojis. Checkboxes are real `- [ ]` boxes. **Add to an existing note before creating a new one**; fewer, fuller notes beat many thin ones.

### Folder indexes (keep them in sync)

Every folder has an index note named after the folder (`<Folder Name>.md`, `type: index`) listing each note with a one-line description. When you create, rename, move or materially change a note, update its folder's index in the same pass. When a new folder is created, create its index at the same time and update the Vault Structure map above.

### Renaming and moving notes

Moving a note between folders is safe (links follow the note name); update both folder indexes. Renaming breaks links unless it is done inside Obsidian. If you rename a file directly, fix every `[[old name]]` link by hand.

### Saving (checkpoints)

Whenever something changes that a future session would need, save it the same turn: the note it belongs in, today's daily note, and (only for a new always-on rule) AGENTS.md. **A daily-note entry alone is never the record.** Then check the touched folder's index for drift and fix it.

### Archiving

When I say something is done or ask to archive a note: set `status: archived`, move it to `06 - Archive` with the same name, and tell me what moved. Never archive on your own.

### Writing rules

- **No em-dashes in anything I'll post or send** (posts, emails, replies, flyers). They read as "an AI wrote this".
- Customer and vendor replies are short, warm and sound like me.
- [FILL IN: your own writing rules, or delete this line.]

### Daily Notes

Daily notes record what happened across all my sessions for a day. They live in `01 - Daily Notes/`, in month folders named `NN - Month YYYY` from the very first note, filename `YYYY-MM-DD.md`, frontmatter `status: active`, `project: business`, `type: log`. Create every one from `01 - Daily Notes/Daily Note Template.md`. If today's note exists, add a new session section and a line in its Index; don't overwrite. Use my local time.

**When I say I'm done** ("that's it for today", "goodnight"), offer to update today's note. Check the real date and time first.

**At the start of a conversation,** after this index, check yesterday's note. If it's missing and you know what happened, create it and say it's rebuilt and may be incomplete; if nothing happened, skip it. If it exists and you know something it's missing, add a session section.

### Living profile

Update the profile sections (Key People, How I Work, Daily Routine) quietly as you learn new things, and log each change in the daily note under "Profile Updates". Don't change Who I Am, My Business, How I Like to Work with the AI, or these Vault Rules; only I change those. A passing mention isn't a trait; fewer, better updates.
