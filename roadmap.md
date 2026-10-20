# WebCraft roadmap

## Landing redesign
- [x] Redesign the entire landing page and animated 3D composition.
- [x] Remove credit-card and free-forever claims; verify navigation and template selection.

## Fix list (from Gabriel)

- [x] Create-project-from-template flow — verified end to end: sign in → Templates → Use template → project opens with all template blocks on the canvas.
- [x] Pages feel like real pages — pages panel with Home/Team chat, blank-page creation, per-page export and publish.
- [x] Real-time code viewer — Code tab regenerates HTML/CSS/JS on every canvas change (verified: editing block text updates the code instantly); manual edits still preserved until reset.
- [x] Builder blocks customizable and functional — per-block text, link, style, attributes, layout and logic editing verified working.
- [x] Email/password login + register alongside Google — both work; email confirmation is now auto-confirmed so accounts sign in immediately.
- [x] Container blocks are real layout panels — drop any block onto a Flex row / Grid / Stack / Absolute box / Section to nest it; children move/resize inside the container, export nests the HTML, thumbnails render nesting, deleting a container deletes its children.

## Round 3 (import + fixes)
- [x] Import GitHub project, move database/users to Lovable Cloud
- [x] Photos & videos show in editor, preview, published site, ZIP and one-click deploys (upload + bundled media)
- [x] Friendly "Behaviour & accessibility" settings replace raw attributes (advanced kept tucked away)
- [x] One-click publish to Netlify / Vercel free plans
- [x] Layout panels (flex, grid, stack, absolute, section) enforce real layout; section is a pure panel with a hint
- [x] HTML / CSS / Script snippets for every block type; new blocks arrive pre-styled like template blocks

## Device support
- [ ] Adapt workspace and editor for phones and tablets; enforce phone viewing-only access and verify.

## Backlog (deferred)

- [ ] Revision history + rollback UI (activity table already stores before/after)
- [ ] Inline text editing directly on the canvas
- [ ] Publish to a friendly subdomain
- [ ] Live theme sync across open tabs
- [ ] Drag an existing block into/out of a container (currently nesting happens on drop from the palette)
