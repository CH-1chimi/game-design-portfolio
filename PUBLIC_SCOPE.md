# Portfolio tool suite: scope and refactor plan

20 October 2026 · public-safe first pass

## Source audit and release decision

- **Universal Combat Lab v0.8.2**: generic, synthetic reference implementation with documented game-reference formula caveats and no embedded build dataset. Included as a working standalone browser app with an added portfolio return bar. Its existing calculator, baseline storage, analytics, CSV/JSON export and A/B battle code is preserved.
- **Coin Economy Editor v24**: source includes embedded multi-scenario reward, stage and build-reference records, and a bot bridge. It is NOT published. The portfolio demonstrates the reusable design question with new synthetic values, anchor editing, reward and price curves, and a separate demo-only JSON export.
- **Unit Benchmark / Balance Lab**: source includes very large embedded unit, skill and art datasets. It is NOT published. The portfolio uses independently written simplified HP/ATK growth, derived CP and flat-defense inspection; public demo export only.
- **1085 Bot Generator**: source includes APK-derived progression, unit/enemy records, lineups and a private economy/unit import contract. It is NOT published. The portfolio demo imports only the two independently reconstructed demo schemas and visualizes a simplified progression-to-enemy-target chain.

## Visitor walkthrough

1. In `tools/economy-demo.html`, adjust the stage reward anchor and summon inflation; export the public economy JSON.
2. In `tools/unit-demo.html`, adjust HP and ATK growth; export the public unit JSON.
3. In `tools/progression-demo.html`, import both demo JSON files, inspect stage power and export a stage CSV.
4. Open `tools/universal-combat-lab.html`, select a formula, capture a baseline under Balancing Workspace, then use Analytics or A/B Battle.

## What should come next

- Replace the simple economy demonstration with a more expressive but still synthetic pacing model: configurable source types, stage unlock annotations and editable anchors.
- Extend the unit demonstration to multi-rank and skill growth, meaningful role comparison and traceable CP breakdown.
- Upgrade the progression demonstration to configurable, fictional roster composition and wave layouts, then test end-to-end with generated demonstration fixtures.
- Author editorial case studies: the design problem, contribution, constraints, validation decisions and outcomes for each tool.
- Perform final employer confidentiality review before publishing any screenshots of original builds or claiming attributable retention/performance results.

## QA performed

Browser interaction checks against inline renderings in Chromium: public editor input updates, demo exports, cross-demo imports, estimator CSV export, UCL baseline capture and A/B run, desktop layout and 390px mobile width. There were no page-script errors or viewport horizontal overflows in those cases. These checks do not constitute a complete test of every feature in the supplied UCL source.

The production/private import schemas are intentionally incompatible with all public demo files.

User-provided character art for Summer Sniper Physalis and Rain (NV / Brave Shift) and original public DigiPen screenshots are presentation-only public references; they are not claims of sole authorship.

Media provenance update: Legion Attack! and Road Busters use user-supplied public video thumbnails. My Food Factory links to its public gameplay video and Google Play store, with optional remote store screenshot and clearly labelled local fallback. No confidential economy source data added.

My Food Factory media: locally archived, user-provided 1152×2048 public promotional image and a 16:9 upper gameplay crop. No production source assets or private economy data added; no live Google Play image dependency.
