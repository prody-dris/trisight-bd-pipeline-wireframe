# HEARTBEAT.md — TRISight BD Pipeline Wireframe

> Shift handoff log for this wireframe repo. Update at the end of every working session that touches it.

---

## 2026-06-30 — BD Pipeline Kanban with stage-pick popup (PR #4, merged)

**Done:**
- Added an interactive **Pipeline Kanban** view to `index.html` (+605/-3). Merged via PR #4 (commit `b943347`).
- 8 BD-stage columns (`custom_bd_pipeline` order), draggable proposal cards (13 demo proposals). Dragging into a column that maps to >1 detailed `stage` opens a popup to pick the sub-stage; earliest sub-stage pre-selected so the user usually just confirms. Other columns move silently. Cancel reverts to origin column.
- **Fan-out columns** (popup fires): Proposal (3), MOU (3), Initial Conversation/ Pitching (2), Concept Note (2) — derived from the live `tri` stage→BD mapping, read in reverse.
- **3 popup variants** behind a toggle, same board + data: A centered modal · B inline `<select>` on the card · C right slide-in panel with proposal context + source→target flow.

**Pending:**
- Pick the winning popup variant (A/B/C); strip the other two in a follow-up.
- Confirm GitHub Pages build finished; verify at https://prody-dris.github.io/trisight-bd-pipeline-wireframe/.

**Blocked:**
- None.

**Decisions:**
- **Wireframe flips the live direction.** Live `tri` derives BD stage FROM the detailed `stage` (client script). This kanban makes BD the input and detailed the output. Fine for a wireframe; the real build must resolve which field is master.
- **Popup fires on any fan-out column (>1 sub-stage), all 4** — not just Proposal/MOU. Earliest sub-stage as the prefilled default.

---

## 2026-06-30 — Merged PR #2 (BD Pipeline & Grants wireframe per TRIF feedback)

**Done:**
- Merged PR #2 into `main` (merge commit `22c5b29`); head branch `wireframe-updates-bd-grants-funnel` deleted.
- `index.html` only, +190 / −156. Implements TRIF review feedback:
  - **BD Pipeline:** relabels (Largest in Pipeline → Highest Valued Proposal; Stalled → Proposals Awaiting Action); description/tooltip rewrites; Stage Distribution glossary moved above the chart, Grant Anchor + Funds added to drill-down; funnel consolidated to 8 stages (MoU WIP + MoU Signed merged into MOU across data, chart, kanban, list, glossary).
  - **Grants Dashboard:** Total/Active Grants descriptions updated; "MoU yet to be attached" card folded into Profiling Pending; Profiling Pending moved into Grants Overview; clickable per-state Geographic Distribution drill-down with District/Block columns, data-driven markers, multi-state grants under each state, legend overlap fixed.

**Pending:**
- Confirm GitHub Pages build finished; verify live page at https://prody-dris.github.io/trisight-bd-pipeline-wireframe/.

**Blocked:**
- None.

**Next:**
- Share live link with TRIF / Brahmjyot if this is the intended publish.

**Decisions:**
- **Merge commit, not squash** — preserved the single authored commit and Brahmjyot↔Claude co-author trail for the audit record.
