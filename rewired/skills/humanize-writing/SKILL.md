---
name: humanize-writing
description: Apply to ALL prose writing and content output — every draft, email, article, LinkedIn post, bio, pitch, report, or edit of existing text. This skill strips the statistical fingerprints of AI writing so output reads like a sharp human wrote it. ALWAYS load this skill before producing any prose deliverable, even short ones, and even when another skill (like email-drafting) is also in use — this skill governs the sentence-level style underneath all of them. Triggers include any request to write, draft, rewrite, punch up, edit, humanize, or "make this sound less AI."
---

# Humanize Writing

Every LLM regresses to the mean: it swaps specific, unusual facts for generic, important-sounding ones. The portrait gets louder while the photo gets blurrier. This skill reverses that. The goal is not "avoid a word list" — it's to write with the specificity, asymmetry, and restraint that statistical text generation naturally sands away.

Work through three passes: **substance**, **structure**, **sentence**. Then run the final checklist.

## Pass 1: Substance (the deep tells)

These matter most. Fixing vocabulary while leaving these in just makes detection harder without making writing better.

**No inflation of significance.** Never tell the reader something matters, represents a shift, marks a moment, underscores importance, reflects broader trends, sets the stage, leaves an indelible mark, or cements a legacy. Show the specific fact and let it carry its own weight. "She booked 47 keynotes in 2025" beats "She has established herself as a pivotal voice."

**No superficial analysis bolted onto facts.** Kill the trailing "-ing" clause that interprets the sentence you just wrote: "...launched in March, signaling a new era" / "...grew 40%, reflecting strong demand." State the fact. If the interpretation matters, give it its own sentence with an actual argument behind it.

**No vague authority.** No "experts argue," "observers note," "industry reports suggest," "many believe." Either name the source or own the claim yourself.

**No hedged filler.** Cut "it's important to note," "it's worth mentioning," "keep in mind that." If it's important, saying it is the proof.

**No canned arc.** No "Despite challenges... continues to thrive." No Challenges section, no Future Outlook, no "In conclusion" paragraph that restates what was just said. End on the strongest specific point, not a summary.

**Specifics over adjectives.** Every time you reach for "innovative," "renowned," "groundbreaking," "world-class," replace it with the fact that would make a reader think that word themselves.

## Pass 2: Structure

**Break the rule of three.** LLMs default to triplets: three adjectives, three parallel phrases, three bullet groups. Vary it. Use one item, or two, or four. If a triplet survives, it should be because those are genuinely the three things.

**No negation parallelism.** Banned in all forms: "It's not X, it's Y." "Not just X, but Y." "This isn't about X — it's about Y." "X rather than Y" as a reflexive pattern. Say the true thing directly without first knocking down a strawman.

**Prose over formatting.** No bullet lists with bolded inline headers ("**Speed:** the system is fast"). No headers on short pieces. No bolding for emphasis scattered through paragraphs. Bold nothing unless the format genuinely demands it (and it almost never does).

**Vary sentence length for real.** Not mechanically — but a paragraph where every sentence is 18-24 words with a subordinate clause is a machine pattern. Let some sentences be four words. Let one run long when it earns it.

**Repetition is fine.** Calling the same thing by the same name twice in a paragraph is human. Elegant variation ("the company... the firm... the organization... the enterprise") is a repetition-penalty artifact. Pick the natural word and reuse it.

**Sentence case for any headings.** Never Title Case Every Main Word.

## Pass 3: Sentence-level style

**Use "is," "has," "was."** LLMs avoid plain copulas. Write "is" instead of "serves as," "stands as," "functions as," "represents." Write "has" instead of "boasts," "features," "offers," "maintains." Write "was a candidate" instead of "ventured into politics as a candidate."

**Plain verbs.** wrote (not authored), used (not utilized), moved (not relocated), tried (not attempted), showed (not demonstrated or showcased), started (not embarked upon), died (not passed away).

**Punctuation.** No em dashes, ever. Use commas, periods, colons, or parentheses. Straight quotes and apostrophes, not curly. No emoji as formatting or bullet decoration.

**Superlatives and hedges are allowed.** Humans write "one of the best," "the only," "very," "perhaps," "tends to." Don't scrub these — their absence is itself a tell.

**Contractions.** Use them wherever a person speaking would.

For the full banned-vocabulary list and phrase-level substitution table, read `references/ai-tells.md` — do this whenever editing or rewriting existing text, since the list is long and specific.

## Final checklist (run on every output)

1. Search the draft for any word in the banned list (references/ai-tells.md). Replace with plain alternatives or cut.
2. Zero em dashes. Zero "not X, but Y" constructions. Zero trailing "-ing" analysis clauses.
3. Zero sentences that assert importance, significance, legacy, or broader trends without a concrete fact doing the work.
4. Count the triplets. If more than one rule-of-three survives per ~300 words, break some up.
5. Read the last paragraph. If it summarizes or restates, delete it and end one paragraph earlier.
6. Read one paragraph aloud (mentally). If no human would say any sentence in it out loud, rewrite that sentence.
7. Verify formatting restraint: no unnecessary bold, no inline-header bullets, no Title Case headings, no emoji.

## What this skill does NOT mean

Don't overcorrect into fake-casual sloppiness, forced slang, or deliberate typos. Don't strip personality, strong claims, or rhythm. The goal is the user's natural voice: confident, direct, and specific. The target is writing that a smart, busy person wrote fast because they knew exactly what they meant — not writing that's trying to pass a detector.
