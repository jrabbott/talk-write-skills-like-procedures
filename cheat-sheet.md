# STE for agent skills — cheat sheet

*ASD-STE100 spirit for `SKILL.md` writers. Not a full STE course. No clause numbers.*  
*Clearer procedures help agents follow — and are easier for humans to scan too.*  
*Paste into chat, pin in the channel, or drop on a closing slide.*

---

## STE → skill rules

- Skills are **procedures** — write steps an agent can execute.
- Use a **small skill-local glossary**; pick one word per concept.
- **One word, one meaning** (don’t overload `run`, `project`, `handle`).
- Prefer **short imperative sentences**: `Read…` / `Create…` / `Verify…` / `Do not…`
- One action per step; number the order.
- Separate **hard** rules (`must` / `do not`) from **soft** ones (`prefer` / `if needed`).
- Keep exact tokens: flags, paths, API names, error strings.
- Shape: **When to use → Terms (optional) → Steps → Do not**.

---

## Do

- Write the happy path, then short “If this fails…” exits.
- State a **done-state** (what “finished” looks like).
- Stop early on failure; say what to report.
- Reuse the same term for the same object end-to-end.

## Don’t

- Vague verbs: *ensure*, *handle*, *consider*, *be mindful*, *appropriately*.
- Synonym drift: *repo / codebase / project / tree* for the same thing.
- Nested *if / unless / except* in one sentence.
- Mix soft suggestions into hard steps.
- Invent STE dictionary entries or fake rule numbers.

---

## Mini before → after *(synthetic)*

**Before**
> If the user asks for a deploy, unless they only wanted a dry run (except in production where you should always confirm), try to deploy and handle issues.

**After**
> 1. If dry run only: run dry-run. Report. Stop.  
> 2. If production: get explicit confirmation. Do not deploy before confirm.  
> 3. Deploy the named target.  
> 4. On failure: report command + error. Do not claim success.

---

## CTA

Tonight: rewrite **one** skill’s **Steps** + **Do not** in this style. Run it twice on the same task. Keep what made following more consistent — for the agent, and for the next human who reads the skill.
