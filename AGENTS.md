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

- Keep real catalogue entries in `src/lib/products.ts` with uploaded-media asset pointers; this prevents dummy data and repeated media from returning.
- Use the dedicated Radix dialog and react-zoom-pan-pinch product viewer for product images; maintained libraries provide modal accessibility and cross-device gestures.
