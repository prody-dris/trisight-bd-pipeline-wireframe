# HEARTBEAT.md — TRISight BD Pipeline Wireframe

> Shift handoff log for this wireframe repo. Update at the end of every working session that touches it.

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
