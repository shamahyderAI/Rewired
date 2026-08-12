# AI tells: banned vocabulary and phrase substitutions

Distilled from Wikipedia's "Signs of AI writing" field guide. These words and constructions are statistically overrepresented in LLM output. One instance may be coincidence; clusters are a fingerprint. Default action: replace with the plain alternative or cut entirely.

## Banned words (replace or cut)

| Banned | Use instead |
|---|---|
| delve | dig into, look at, explore (or just state the thing) |
| tapestry (abstract) | cut; name the actual components |
| landscape (abstract) | market, field, industry, or cut |
| testament / a testament to | shows, proves (or cut and show the fact) |
| underscore(s) | shows, makes clear (usually cut) |
| highlight(s) (as verb of significance) | shows, or restructure |
| showcase / showcasing | shows, displays |
| pivotal | key fact stated plainly, or cut |
| crucial | important, or cut |
| vital | important, or cut |
| robust | strong, solid, or specific spec |
| vibrant | specific detail instead |
| intricate / intricacies | detailed, complex, or specifics |
| meticulous(ly) | careful(ly), or cut |
| boasts | has |
| fosters / fostering | builds, creates |
| garner(ed) | got, won, earned |
| bolster(ed) | strengthen, support |
| enduring | lasting, or cut |
| enhance / enhancing | improve, or specifics |
| leverage (verb) | use |
| utilize | use |
| embark(ed) | start(ed) |
| journey (metaphorical) | career, process, work, or cut |
| navigate (metaphorical) | handle, manage, deal with |
| realm | field, area, or cut |
| interplay | relationship, or restructure |
| seamless(ly) | smooth, easy, or cut |
| holistic | complete, whole, or cut |
| elevate (metaphorical) | improve, raise |
| empower(ing) | give/let (people do X) |
| unlock (metaphorical) | open up, enable, or restructure |
| harness (metaphorical) | use |
| groundbreaking | new, first (with the specific) |
| renowned | known for [specific thing] |
| nestled | in, located in |
| in the heart of | in, in central [place] |
| valuable insights | what was actually learned |
| align(s) with / resonate(s) with | fits, matches, or restructure |
| evolving landscape | cut entirely |
| focal point | center, main point |
| indelible mark | cut; state what changed |
| deeply rooted | old, longstanding, or specifics |
| key (as adjective, overused) | main, or cut |
| notably (sentence opener) | cut |
| additionally (sentence opener) | also, and, or restructure |
| moreover / furthermore | also, or just start the sentence |
| comprehensive | full, complete, or cut |
| myriad | many, or a number |
| plethora | many, plenty |
| ever-evolving / ever-changing | cut |
| game-changer / game-changing | state what changed |
| cutting-edge | new, latest, or the specific tech |
| state-of-the-art | newest, best available, or specifics |

## Banned phrases and constructions

**Significance inflation (cut the whole clause):**
- "stands as / serves as a [testament/reminder]"
- "plays a [crucial/pivotal/vital/key/significant] role in"
- "marks a [pivotal/significant] [moment/shift/turning point]"
- "underscores/highlights its [importance/significance]"
- "reflects broader [trends/movements/debates]"
- "symbolizing its [ongoing/enduring/lasting]..."
- "setting the stage for" / "shaping the" / "contributing to the broader"
- "has generated debate about" / "has prompted broader reflection on"
- "solidified its role as" / "cemented its place as"

**Copula avoidance (rewrite with is/has/was):**
- "serves as" → is
- "stands as" → is
- "functions as / operates as" → is
- "represents a" → is a
- "boasts / features / offers / maintains a" → has a
- "holds the distinction of being" → is
- "refers to" (in a lead/definition) → is
- "began his career as" → was (when that's what's meant)

**Fake-secret framing (cut the whole line; state the point directly):**
- "Here is the part almost nobody discusses"
- "What nobody's talking about is..."
- "Nobody talks about this, but..."
- "The part everyone misses"
- "What no one tells you about..."
- "...that no one is talking about"
These manufacture insiderness instead of earning it. If the point is genuinely under-discussed, the content will make that obvious; announcing it is the tell.

**Superficial analysis (cut the trailing clause):**
- "..., highlighting/underscoring/emphasizing [significance]"
- "..., ensuring [outcome]"
- "..., reflecting/symbolizing [meaning]"
- "..., contributing to [broader thing]"
- "..., cultivating/fostering [quality]"
- "..., demonstrating [importance/relevance]"
- "..., signaling [shift/new era]"

**Vague authority (name the source or own the claim):**
- "experts argue / observers have cited / some critics argue"
- "industry reports suggest"
- "widely regarded as / widely interpreted as"
- "several sources note" (when citing one or none)
- "is described in scholarship as"

**Hedged filler (cut):**
- "it's important/worth noting that"
- "it's crucial to remember"
- "keep in mind that"
- "In summary / In conclusion / Overall," (as closer)

**Canned arcs (delete and restructure):**
- "Despite [challenges], [subject] continues to [thrive/grow/adapt]"
- "Despite these challenges..."
- Any "Challenges," "Future Outlook," or "Looking Ahead" section
- Final paragraphs that restate the piece

**Negation parallelism (all banned, standing brand rule):**
- "It's not X, it's Y" / "It's not just X — it's Y"
- "Not only X, but also Y"
- "This isn't about X; it's about Y"
- "No X, no Y, just Z"
- Reflexive "X rather than Y"

**Chatbot residue (never appears in final output):**
- "I hope this helps" / "Would you like me to..." / "Let me know if..."
- "Certainly!" / "Of course!" as openers
- Any meta-commentary about the writing itself

## Formatting tells (never)

- Em dashes (—) in any position
- Curly quotes/apostrophes when the platform doesn't force them
- Title Case Headings
- Bold inline-header bullets ("**Speed:** it is fast")
- Emoji as bullets or heading decoration
- Markdown artifacts (asterisks, ##) in plain-text deliverables
- Horizontal rules between sections of short pieces

## Allowed (do not scrub these; their absence is a tell)

- Superlatives: "one of the best," "the first," "the only"
- Hedges and intensifiers: "very," "perhaps," "tends to," "probably"
- Plain wordiness: "as a result of," "in order to," "the fact that"
- Repeating the same noun instead of rotating synonyms
- Starting sentences with And, But, So
- Contractions everywhere
- Strong first-person claims
