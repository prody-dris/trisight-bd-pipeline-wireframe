# TRISight — BD Pipeline Wireframe

Clickable static wireframe of the **BD Pipeline** dashboard in TRISight (mGrant NuO, TRI Foundation).
Built for client review and collaborative iteration.

- **Live:** https://prody-dris.github.io/trisight-bd-pipeline-wireframe/
- **Source page:** `/app/bd-pipeline` on the TRISight (mGrant NuO) deployment
- **Stack:** single self-contained `index.html` — no build step, no external JS

## Sections
Filters → Pipeline Overview → Fund Value → Stage Distribution → Pipeline by Stage (bar chart) → Financial Overview → Portfolio Distribution → Lost Opportunity → Stalled Proposals.

All data shown is illustrative (UAT sample). Edit `index.html` directly — sections are marked with `<!-- SECTION N: ... -->` banners and themed via CSS variables in `:root`.
