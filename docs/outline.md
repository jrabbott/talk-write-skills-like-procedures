# Talk outline: ASD-STE100 for agent skills

**Working title:** Write skills like procedures — Simplified Technical English for Cursor agent skills  
**Speaker:** Jon (software engineer)  
**Venue:** remote  
**Audience:** engineers who build agent skills / prompts (`SKILL.md`-style instruction files)  
**Length:** **15 min target**, 25 min absolute max (+10 stretch below)  
**Tone:** practical for builders; personal opening is honest/tool-focused, not inspirational-keynote  
**Must include:** before/after skill rewrites (primary content block)  
**Examples:** **synthetic only** (no real or sanitized production skills)  
**Opening:** personal backstory (dyslexia → LLMs → STE100)  
**Handout:** [`cheat-sheet.md`](../cheat-sheet.md) — paste into chat or share as slide/PDF after

---

## Primary path — 15 minutes

| Section | Time | Role |
| --- | --- | --- |
| 0. Personal backstory + “how STE helps” + thesis | **~3–3.5 min** | Protected — story → read/write examples → bridge → thesis |
| 1. STE → skill mapping (brief) | **~2 min** | Trimmed — four conventions only; no re-telling the bio |
| 2. Before/after rewrites | **~6.5–7 min** | **Largest block — required; synthetic** (do not steal from here) |
| 3. Risks (very short) | ~1 min | Protected — one slide |
| 4. CTA | **~1.5 min** | Protected (+ cheat sheet in chat) |
| Chat Q&A | after talk / leftover | Remote: questions in chat, not mid-flow |

**Timing tradeoff (document for Jon):** personal open costs ~1–1.5 min vs an impersonal hook. Paid for by trimming mapping (~3 → ~2) and CTA (~2 → ~1.5). Before/after stays **~6.5–7** — still the largest block. If §0 runs long, cut mapping anti-pattern line and Example A teaching beat — **never** cut Example C or CTA.

**Hard cuts for 15:** long dyslexia memoir, STE history, full anti-pattern lecture, 8-item convention list, live audience rewrite, tooling wishlist.

---

## Remote delivery notes (whole talk)

- **Screen share:** share slides only (or a single markdown pane). Don’t flip between apps mid-example.
- **Readable diffs:** before/after on one slide, large type; prefer “Before” → “After” columns. Label each slide **Synthetic example**. No tiny full-file walls of text.
- **Pace for remote:** pause 2 seconds after revealing each After so people can read.
- **Chat Q&A:** say up front — “Drop questions in chat; I’ll take 1–2 at the end if time.” Don’t open the floor mid-before/after.
- **Bandwidth fallback:** if screenshare lags, paste Example C (shortest nested rewrite) into chat and narrate.
- **Mute discipline:** stay on mute-friendly delivery — no “any questions so far?” loops that burn the 15.
- **After CTA:** paste link/text of `cheat-sheet.md` into chat.

---

## 0. Personal backstory + how STE helps + thesis (~3–3.5 min)

Personal and honest — coping tools, not pity or keynote inspiration. Engineers respect concrete mechanics.

### Arc (keep this order)

1. Dyslexia / reading–writing as chore (~30–40s)  
2. LLMs: heart sank — “language” in the name (~20–30s)  
3. STE100 love + **how it helps read & write** (~60–75s)  
4. Bridge → skills are procedures + thesis (~45–60s)

### Suggested first-person script *(Jon: edit to your voice)*

> I’ve got dyslexia. Reading and writing have always been a challenge — honestly, a chore. Engineering clicked; long prose never did.  
> Then AI showed up. LLMs — the clue’s in the name: **language**. My heart sank. The job suddenly meant more prompts, more skill files, more synonym-heavy instructions. The hard part was doubling down.  
> What helped me is ASD-STE100 — Simplified Technical English. I love it. It makes language work tractable for me when I’m **reading** and when I’m **writing**.  
> [Deliver 2 reading + 2 writing examples from the draft list below — not all six.]  
> Here’s the bridge: if constrained language helps a human reader like me, it also helps an agent that follows instructions under ambiguity. Same enemy — foggy prose. Same fix — clear words, clear steps.  
> Agent skills are **procedures**, not prompt poetry. Tonight: a few STE→skill rules, synthetic before/afters, then try one skill yourself.

### How STE helps — draft examples

**⚠️ Draft — Jon should personalize.** Plausible lived-experience beats for rehearsal; swap in your real moments so we don’t invent false autobiography. In the 15-min path, speak **two reading + two writing** max.

**Reading (pick 2)**
1. **One word, one meaning** — I stop re-decoding mid-paragraph whether *run* means execute, session, or go-live. Decode load drops.  
2. **Short numbered steps** — I can hold one action in working memory. Nested “if/unless/except” sentences are where I lose the thread.  
3. **Stable terms** — skimming doesn’t mean hunting *repo / codebase / project / tree* for the same thing; my eyes can track the procedure.

**Writing (pick 2)**
1. **Imperative template** — *Do X. If Y, stop. Do not Z.* beats staring at a blank skill file trying to “sound smart.”  
2. **Limited / local vocab** — I’m not synonym-hunting among five fancy words; I pick the house word and move on.  
3. **Hard vs soft separated** — I stop burying the real rule under “should generally try to…,” which used to be how I hedged when writing felt risky.

### Thesis close for §0

- Familiar agent failure (one line): wrong synonym / skipped nested unless / soft verb treated as optional.  
- Thesis: STE spirit → `SKILL.md`. Agenda: rules → synthetic rewrites → limits → CTA + cheat sheet.

**Speaker notes (remote)**
- First person throughout this section; then switch to “we / you” for the craft.
- Slide: one line only — “Dyslexic engineer. STE made language tractable. Skills need the same.” No bio deck.
- Say “Simplified Technical English (ASD-STE100)” once, then “STE.”
- Cap story + examples at ~3 min; if behind, drop to 1 read + 1 write example and jump to thesis.
- Tone check: tool that works, not overcoming narrative. If chat reacts to dyslexia, acknowledge once; park deeper Qs for after.
- After thesis, flash synthetic bad snippet (large font) — explain in §2.

---

## 1. STE → skill mapping, brief (~2 min)

You’ve said *why you* care. Now *why skills* care — no bio callback longer than one sentence.

**Talk point — STE spirit in one breath**
- Controlled language: limited vocabulary, **one word / one meaning**, short sentences, imperative steps.
- Not certification; not memorizing the dictionary. Adopt the discipline.
- One-sentence callback: same habits that help me read/write help agents follow.

**Talk point — why skills care**
- Skills are operational: when to load, what to do, what not to do, in order.
- Ambiguity → variance in agent following. STE-shaped writing buys **consistency**, not “smarter models.”

**Talk point — four conventions (only these in 15)**
1. **Skill-local terms** — small glossary; no synonym drift (`repo` / `codebase` / `project`).
2. **One meaning per word** — if `run` means “execute the command,” don’t also mean “chat turn.”
3. **Short imperative steps** — one action per sentence; numbered order.
4. **Hard vs soft isolated** — `must` / `do not` mean it; park `prefer` separately.

**Anti-patterns (one breath)**
- Vague verbs: ensure / handle / consider. Nested if/unless/except. Soft rules mixed into hard steps.

**Speaker notes (remote)**
- One slide: four bullets. Don’t re-list the personal read/write examples here.
- Unsure of an STE clause number → “STE spirit / approximate.” No invented dictionary entries.

---

## 2. Before / after rewrites (~6.5–7 min) — required, largest block

**Source:** all examples below are **synthetic** `SKILL.md` fragments invented for this talk. They are not from a real skill. They illustrate STE *spirit* only — not claimed STE dictionary citations or clause numbers.

**In 15:** deliver **A (~2–2.5 min) + C (~3.5–4 min)** fully; keep **B** as backup if A lands under 2 min. Teaching beat: Before → what the agent can misread → After → which ambiguity died. If §0 ran long, shorten A’s “ambiguity that dies” line — keep C intact.

### Example A — vague verb → imperative + done-state (~2.5 min)

*Synthetic · skill fragment: “Setup” steps*

**Before**
> Before you change anything, ensure the environment is set up correctly and be mindful of missing dependencies. Handle install problems appropriately so the rest of the skill can proceed smoothly.

**After**
> ## Steps — setup  
> 1. From the repository root, run the project install command.  
> 2. Run the project typecheck (or tests if there is no typecheck).  
> 3. If install or typecheck fails, stop. Report the failing command and the error.  
> 4. Do not edit feature files until install and typecheck succeed.

**Ambiguity that dies:** “ensure / be mindful / handle appropriately” → concrete commands, stop condition, and a clear done-state.

### Example C — nested conditional → ordered steps + early stop (~3.5 min)

*Synthetic · skill fragment: “Deploy” steps — lead example; also on the cheat sheet*

**Before**
> If the user asks for a deploy, unless they only wanted a dry run (except in production where you should always confirm), try to deploy and handle issues. Prefer not to bother them unless necessary.

**After**
> ## Steps — deploy  
> 1. If the user asked for a dry run only: run the dry-run command. Report the result. Stop.  
> 2. If the deploy target is production: ask for explicit confirmation. Do not deploy before the user confirms.  
> 3. Run the deploy command for the named target.  
> 4. If deploy fails: report the failing command and the error. Do not claim success.  
> 5. Do not retry a failed production deploy with different flags unless the user asks.

**Ambiguity that dies:** nested unless/except, soft “try / prefer / handle,” missing stop points → ordered early exits and hard `do not`s.

### Example B — synonym soup → one term (backup / stretch)

*Synthetic · skill fragment: “Edit” steps*

**Before**
> Open the repo, inspect the codebase, and update the project tree so the application reflects the change. Keep the workspace consistent.

**After**
> ## Steps — edit  
> 1. Open the repository root.  
> 2. Find the files for this change.  
> 3. Edit only those files.  
> 4. Verify the app shows the change.  
> 5. Do not rename “repository” to “codebase,” “project,” or “tree” in this skill — use **repository** only.

**Ambiguity that dies:** repo / codebase / project / tree / workspace → one house term.

**Speaker notes (remote)**
- Say once: “These are synthetic fragments — not a real skill.”
- Screen-share diffs at **slide-readable size**; label **Synthetic**.
- Pattern: read Before → name the failure mode → reveal After → one line on what died.
- Stress: shorter is not the goal — **unambiguous action** is. After can be longer.
- No live audience rewrite in the 15.

---

## 3. Risks — very short (~1 min)

**Talk point (one slide, three lines)**
- **Too rigid:** exploratory/design skills, or drafts where the procedure isn’t stable yet.
- **Keep exact tokens:** CLI flags, paths, API names, error strings — don’t “simplify” proper nouns.
- **No full STE checker for skills yet:** lint by convention (terms, vague verbs, Steps / Do not).

**Speaker notes (remote)**
- Do not open the tooling rabbit hole; point chat questioners to “after talk.”
- Honest closer line: discipline, not a silver bullet for missing evals.

---

## 4. Takeaways + CTA (~1.5 min)

**Takeaways (3 bullets on slide)**
1. Skills are procedures — write them that way.  
2. STE spirit: constrained words, one meaning, short imperatives → more consistent agent following (and clearer for human readers too).  
3. Kill vague verbs and nested exceptions first.

**Call to action**
- Tonight: pick **one** skill. Rewrite only **Steps** and **Do not** into STE-like imperatives. Run it twice on the same task. Note whether following got more consistent.
- Optional: add a 5–10 word Terms list at the top.
- Handout: paste [`cheat-sheet.md`](../cheat-sheet.md) into chat (or share as PDF/slide).

**Close**
- Optional one-beat callback: “STE made language workable for me. Same discipline makes skills workable for agents.”
- Then: “Don’t write skills to sound smart. Write skills so the agent can’t misunderstand the next action.”
- Reminder: “Questions in chat — I’ll grab what I can.”

**Speaker notes (remote)**
- CTA slide stays up during any leftover Q&A.
- Drop the CTA + cheat-sheet path/text in chat as you say it.
- Don’t reopen the personal story at the end unless chat asks — protect the action.

---

## Optional +10 stretch → 25 min max

Use only if the slot allows. Add in this order; stop at 25. All stretch examples stay **synthetic**.

| Add | Time | What |
| --- | --- | --- |
| Example B (synonym soup) | ~2 min | Full treatment, not backup |
| Example D — soft/hard mix | ~2 min | See below |
| Anti-pattern → symptom mini-table | ~2 min | Synonyms / nested ifs / vague verbs / soft+hard |
| Mapping depth | ~2 min | Obligation levels, done-states, section shape (When → Terms → Steps → Do not) |
| Extra personal example (from draft list) | ~1 min | Third read or write example Jon didn’t use in §0 — only if energy is there |
| Chat Q&A (curated) | ~2 min | Answer 2–3 typed questions; skip open mic |

### Example D — soft/hard mix (stretch only)

*Synthetic · skill fragment: “Edit this skill”*

**Before**
> You should generally prefer editing the skill, and make sure not to break things. Feel free to tidy other files if it seems helpful.

**After**
> ## Steps  
> 1. Edit only the skill file the user named.  
> 2. Keep unrelated skills and config unchanged.  
> 3. After the edit, run the skill’s smoke check if one exists.  
> 4. Do not “tidy” other files unless the user asks.

**Stretch rules**
- Do **not** add STE history or aerospace deep-dive.
- Do **not** demo a live checker.
- Do **not** swap in real/sanitized skills.
- If behind at minute 12 of the primary path, **skip the entire +10** — protect CTA.

---

## Slide checklist (remote, 15-min deck)

- [ ] Title + thesis (skills = procedures)  
- [ ] Personal one-liner (dyslexia → STE tractable → skills)  
- [ ] Optional: “How STE helps” — 2 read / 2 write bullets (draft until Jon personalizes)  
- [ ] Hook: synthetic bad skill snippet (large type)  
- [ ] Four STE→skill conventions  
- [ ] Before/after A — labeled Synthetic (readable diff)  
- [ ] Before/after C — labeled Synthetic (readable diff)  
- [ ] Backup: before/after B — Synthetic  
- [ ] Risks: three lines  
- [ ] CTA: rewrite one skill + cheat sheet in chat  
- [ ] Stretch-only: B full, D, anti-pattern table (hidden unless +10)

---

## Locked constraints (resolved)

- Venue: **remote**  
- Length: **15 min target**, **25 max**  
- Audience: **engineers** (skill/prompt builders)  
- Before/after rewrites: **required** (largest block)  
- Examples: **synthetic only**  
- Cheat sheet: **yes** → [`cheat-sheet.md`](../cheat-sheet.md)  
- Opening: **personal backstory** — dyslexia; LLMs felt language-heavy; STE100 helps Jon read & write (with examples); bridge to agent skills
