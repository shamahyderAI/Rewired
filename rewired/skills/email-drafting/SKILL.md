---
name: email-drafting
description: "Draft, reply to, or rewrite emails in the user's own voice. Use when the user asks to draft an email, reply to this, write to someone, help me respond, what should I say to, or pastes or forwards an email thread and wants a response. Also covers subject lines and tone checks on an email they've written. Pairs with humanize-writing for sentence-level style."
---

# Email Drafting

Draft emails that sound like the user wrote them on a good day: direct, specific, human. Not corporate filler, not AI polish. The first draft should be something they could send without editing.

## Step 1: Find the user's voice

Use the best source available, in this order, and stop once you have enough:

1. **What Claude already knows.** The user's saved memory, stated preferences, and any writing-style profile they've set up. Apply it silently.
2. **A voice file.** A USER.md, voice guide, or style notes in the conversation, the project, or a connected folder.
3. **Their sent mail.** If an email tool is connected (Gmail, Outlook, Superhuman, etc.), read three to five recent emails the user sent, ideally to the same person or of the same type. Note greeting, sign-off, length, and how they ask for things. Read only; never change anything in their mailbox during this step.
4. **Nothing yet.** Draft in a plain, direct, warm voice. After the draft, offer once in one line to learn their style from a few sent emails or a short interview. Don't repeat the offer in later emails in the same conversation.

What to pull from any source: tone (casual, dry, warm, formal), typical length, greeting and sign-off habits, phrases they use, things they avoid, and how they handle asks, pushback, and bad news.

## Step 2: Read the situation

**Replying to a thread.** You have what you need. Greet the sender by name, keep the existing subject line, read the whole thread for open questions and prior commitments, and match the thread's formality unless the user wants to shift it. Draft right away.

**A new email.** If the recipient or the core ask is missing, ask for just those in one short, conversational line ("Who's this going to, and what's the main thing you want them to do?"), then draft. If the user gave enough to make a reasonable attempt, draft first and name your assumptions in one line afterward.

## Step 3: Draft

- Concise by default: get in, say the thing, get out. Go longer only when the user asks or the situation needs it (a proposal, a sensitive message, a lot of context).
- Lead with the point or the ask. Put any context after it.
- One clear next step for the recipient, with a date when timing matters.
- No filler: no "I hope this email finds you well," "I wanted to reach out," "please don't hesitate to reach out," or "circling back," unless that is truly how the user writes.
- Apply humanize-writing for sentence-level style.
- Sensitive emails (conflict, bad news, hard feedback): a little warmer and more considered, still short. Say in one line if you softened the tone.
- Negotiations and money: don't state figures, discounts, or commitments the user hasn't given you. Leave a clear [bracket] for them to fill.

## Step 4: Present it

Show the complete email, ready to copy:

```
Subject: [subject line]

[Full email]
```

Don't explain your choices before or after the draft. At most, add one line offering a single adjustment ("Want it shorter or warmer?").

If an email tool is connected and the user asks, you can save the draft into their drafts folder. Never send an email unless the user explicitly tells you to send that specific email.

## Edge cases

- **Several people on the thread:** address the person who needs to act; keep others in mind for tone.
- **Multiple versions requested:** give the best draft first, then one alternative, not five.
- **Very little information:** make a reasonable attempt, then say "I assumed X and Y. Tell me what to change."
