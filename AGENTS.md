<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

- Keep public landing-page styling scoped to its wrapper so redesigns do not change the editor or authentication screens.
- Site media lives in the private `site-media` bucket and is referenced as `/media/<projectId>/<file>` (served by a signed-URL redirect route); template photos are static files in `public/images/` so they work on every origin.
- Exports and external deploys go through `packageSite` in `src/lib/sandbox.ts`, which bundles all media into `assets/` so sites never depend on the editor's origin.
- Database migrations live in `drizzle/migrations/` (the migration tool replays that journal).
