# Decision log

This is a concise, append-only record of durable project decisions. Add new entries at the top. Do not rewrite historical entries; supersede one with a new entry that links to it.

## 2026-09-08 — Make repository state the mandatory chat handoff

**Decision:** `AGENTS.md`, `docs/project-state.md`, and this log are mandatory reading at task start and mandatory updates before task completion.

**Why:** Individual chats retain separate transcripts. Durable project state must be visible to future chats, models, and collaborators without relying on a prior conversation.

**Consequence:** A task is incomplete if it leaves material context only in the chat transcript.

## 2026-09-08 — Frame the research as competing risks, not a price forecast

**Decision:** The initial target is the probability that a qualifying event reaches +20% before -10% within 60 trading days.

**Why:** This corresponds to the practical continuation question while forcing an explicit risk boundary and horizon.

**Consequence:** All baseline labels, metrics, and backtests must report target-before-stop outcomes as well as return distributions.

## 2026-09-08 — Start with interpretable price-only baselines

**Decision:** Build the event panel and price-only / regime-aware baselines before estimates, transcripts, options, or complex models.

**Why:** Added data and model complexity must demonstrate incremental, out-of-sample value.

**Consequence:** Milestone 1 is a data-quality and label-validation milestone, not an ML milestone.

