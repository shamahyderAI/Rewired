---
name: email-drafting
description: >
  Use this skill whenever the user wants to draft, write, reply to, or compose any email.
  Triggers include: "draft an email", "reply to this", "write an email to", "help me respond",
  "compose a message", "what should I say to", forwarding thread context and asking how to reply,
  pasting an email and asking for a response, or any request to communicate via email.
  Always use this skill for email tasks — even quick replies, subject line help, or tone checks.
  Load USER.md before drafting anything so the email sounds like the user, not a template.
---

# Email Drafting Skill

Draft emails that sound exactly like the user — not polished corporate-speak, not robotic AI filler.
Every email should feel like it was typed by a real person who knows what they want to say.

---

## Step 1: Load USER.md

**Before writing a single word of the email, read the user's USER.md file.**

Look for it at:
- `/mnt/user-data/uploads/USER.md`
- `/mnt/user-data/uploads/user.md`
- Any uploaded file named `USER.md` or `user.md`

If USER.md is found, extract:
- **Voice & tone**: How they naturally write (casual, direct, warm, dry humor, formal, etc.)
- **Common phrases or patterns** they use
- **Things they avoid** (filler words, sign-off styles they hate, etc.)
- **Personal context**: Role, relationships, recurring contacts, company/industry
- **Preferences**: Email length defaults, how they handle conflict, how they give feedback

If USER.md is **not found**, proceed but note: "I don't have your USER.md on file, so I'll draft in a neutral-but-human voice. Upload a USER.md to personalize future drafts."

---

## Step 2: Determine Email Type

### Case A — Replying to an existing email
The user has pasted or shown you an email thread. You have everything you need:
- Use the **sender's actual name** in the greeting (not "Hi there" or "Hello")
- Use the **existing subject line** — do not invent a new one
- Read the **full thread** for context: tone set by the sender, outstanding questions, prior commitments
- Match the formality level of the thread unless the user asks to shift it
- Go straight to drafting — no need to ask clarifying questions unless the user's intent is truly unclear

### Case B — New email the user is composing from scratch
**Ask before drafting.** Collect:
1. **Who is this going to?** (name, relationship, context)
2. **What's the core ask or message?** (one sentence is fine)
3. **Any context I should know?** (optional — history, tone, stakes)

Keep the ask short and conversational. Don't present it as a form. Example:

> "Quick questions before I draft — who's this going to, and what's the main thing you want to say?"

Once you have answers, draft immediately.

---

## Step 3: Draft the Email

### Length defaults
- **Default: concise.** Get in, say the thing, get out.
- Only write longer emails if the user explicitly asks, or if the situation clearly warrants it (complex proposal, sensitive situation, lots of context needed).
- Avoid padding: no "I hope this email finds you well", no "Please don't hesitate to reach out", no "Best regards, [Your Name]" unless that's genuinely their style from USER.md.

### Voice rules
- Write from USER.md's voice profile — if they're casual, be casual; if they're dry and direct, be dry and direct
- Use the vocabulary and cadence you observed in USER.md
- Avoid AI tells: no em dashes as a stylistic crutch, no "certainly", no "I wanted to reach out", no unnecessary hedging
- First draft should sound like something they'd actually send without editing

### Structure
- Subject line (for new emails or if re-drafting a reply subject)
- Greeting using the real recipient name
- Body (short by default)
- Sign-off consistent with their style from USER.md

---

## Step 4: Present the Full Draft

Always show the complete, ready-to-send email. Format it clearly so the user can copy it directly:

```
Subject: [subject line]

[Full email body]
```

Do not summarize what you wrote or explain your choices unprompted. Just show the draft.

After the draft, you may offer one brief line like:
> "Want me to make this warmer / shorter / more assertive?"

But keep it minimal — one prompt, not a list of options.

---

## Edge Cases

**Thread with multiple people**: Address the primary sender; CC context comes from the thread.

**Sensitive emails** (conflict, bad news, feedback): Default to a warmer, slightly more considered tone. Still concise — just not abrupt. Flag if you've softened the tone.

**User wants multiple versions**: Draft the default first, then offer variants (e.g., "Here's a softer version if you want it").

**User gives very little info**: Make a reasonable attempt based on what you have, then ask: "I made some assumptions — let me know what to change."

**No USER.md**: Draft in a human, direct voice. Remind them once that uploading USER.md will make future drafts match their actual style.

---

## What Not To Do

- ❌ Don't ask for clarification when replying to a thread — you have the context
- ❌ Don't invent a new subject line when replying
- ❌ Don't pad emails with corporate filler phrases
- ❌ Don't explain your draft before showing it
- ❌ Don't offer five options when one good draft will do
- ❌ Don't forget to read USER.md first
