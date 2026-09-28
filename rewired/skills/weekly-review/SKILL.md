---
name: weekly-review
description: "Use when someone wants to run a weekly review, close open loops, audit stalled projects and commitments, get their system back to trusted, restart a lapsed review habit, or says \"run my weekly review\" or \"help me close out the week\". Walks David Allen's three-phase loop — GET CLEAR, GET CURRENT, GET CREATIVE — with deterministic scripts that inventory open loops, gate the checklist with named gaps, and score commitment health 0-100."
license: MIT
metadata:
  version: 1.1.0
  author: Alireza Rezvani (adapted for Cowork by Rewired)
---

# Weekly Review — GTD Loop → Trusted System

> **Portability:** Reasoning-led skill. Three optional standard-library Python scripts live in the
> `scripts/` folder next to this SKILL.md (call them by that full path). Use them when they help; a
> review run entirely in conversation is just as valid. Evidence comes from whatever the user has
> connected: calendar, email, chat, task tools, or a notes folder on their computer.

## What this does

A personal system is only trustworthy if it gets reviewed — David Allen calls the weekly review
the critical success factor of the whole method. This skill walks the three phases in order and
refuses to call the review COMPLETE while any of the five mandatory GET CURRENT steps is
unaccounted for. Evidence first: scan the workspace for open loops before asking the user to
recall anything, because their memory is exactly what the method says not to trust.

## Phase 1 — GET CLEAR (steps 1-3)

Collect loose inputs, process every inbox to zero (clarify, don't do — anything over two minutes
becomes a next action), then a mind sweep to empty the head. Start with evidence, from whatever is
connected:

- **Calendar:** last week's meetings (promises made in them) and the next two weeks.
- **Email and chat:** threads where the user owes a reply, and threads they're waiting on.
- **Task tools** (Asana, Notion, Linear, etc.): overdue and stale items.
- **A notes folder** on their computer, if one is connected: run the scanner over it.

```bash
# Only when a notes folder is connected: unchecked checkboxes, TODO markers, stale files
python <skill-dir>/scripts/open_loop_scanner.py --dir <connected-notes-folder> --stale-days 14
```

If nothing is connected, run a guided mind sweep in conversation instead: ask about work, people,
money, home and health commitments one area at a time.

Route every loop found to a list — next action, waiting-for, someday/maybe, or trash.

## Phase 2 — GET CURRENT (steps 4-8, all mandatory)

Review the next-action lists (mark done, prune dead), the previous calendar (missed commitments
become actions), the upcoming calendar (prepare, don't react), the waiting-for list (chase or
drop), and every project for exactly one next action. Then check honestly which steps actually
happened. The gate script does this bookkeeping if you want it:

```bash
python <skill-dir>/scripts/weekly_review_gate.py --list   # the numbered ten-step checklist
python <skill-dir>/scripts/weekly_review_gate.py --done "1,2,3,4,5,6,7,8" --skip "9:no someday list yet"
```

A GET CURRENT step that was skipped without a stated reason means the review is incomplete. Say so
plainly and name the missing step.

## Phase 3 — GET CREATIVE (steps 9-10)

Review someday/maybe (activate, keep, or kill), capture new ideas while the head is clear, then
audit the whole commitment portfolio:

List each active commitment with its last movement and its next action. Flag anything stalled,
anything with no next action, and anything that belongs on someday/maybe. For a long list, the
auditor script scores it. Save the list first as a JSON array of
`{"name": "...", "days_since_touched": 3, "has_next_action": true}` objects:

```bash
python <skill-dir>/scripts/commitment_auditor.py --input <commitments.json>
```

Give an overall read (healthy / drifting / overcommitted) and end the review with one named next
action.

## Scripts

| Script | Role |
|---|---|
| `scripts/open_loop_scanner.py` | Inventories unchecked checkboxes, TODO/FIXME markers, and stale files across a directory; grouped counts + per-file locations; `--json`. |
| `scripts/weekly_review_gate.py` | The ten-step three-phase checklist; `--done`/`--skip`/`--list`; completion % + named gaps → COMPLETE (exit 0) / INCOMPLETE (exit 2). |
| `scripts/commitment_auditor.py` | Flags stalled and actionless commitments, computes the 0-100 health score with the formula shown → HEALTHY / DRIFTING / OVERCOMMITTED. |

## References

- [`references/gtd_weekly_review_canon.md`](references/gtd_weekly_review_canon.md) — why the weekly review is the critical success factor; the three-phase structure; cadence discipline (7 sources)
- [`references/open_loop_psychology.md`](references/open_loop_psychology.md) — Zeigarnik effect, plan-making research, attention residue: why open loops tax attention (6 sources)
- [`references/review_cadence_design.md`](references/review_cadence_design.md) — horizons of focus, habit anchoring, timeboxing, failure modes, restart-after-lapse (7 sources)

## Assets

- [`assets/weekly_review_checklist.md`](assets/weekly_review_checklist.md) — fillable three-phase checklist
- [`assets/example_weekly_review.md`](assets/example_weekly_review.md) — a full worked review (scan → checklist → gate → audit → next action)

## Rules

- All five GET CURRENT steps are mandatory; skip only with a stated reason, and the gate still names it.
- Don't call the review complete when a mandatory step was skipped. Name the gap without softening it.
- Process, don't do: during the review, anything over two minutes becomes a next action, not a detour.
- Timebox 60-90 minutes; past two hours, gate what's done honestly and schedule the remainder.
- A lapsed habit restarts with a shorter pass and zero guilt — a review is maintenance, not judgment.

## Distinct From (don't reach for the wrong sibling)

- **morning-brief** — the daily 30-second glance. The weekly review is the deeper maintenance pass behind it.
- **meetings** — extracts action items from one meeting's notes. Feed its output into this review.
- **high-output-management** — for managers reviewing their team's output, not their own commitments.

---

**Version:** 1.1.0 · **Credits:** Alireza Rezvani (MIT), adapted for Cowork by Rewired.
