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

## Game architecture
- Preserve the imported browser Canvas RPG engine and original catalog; settlement mechanics live in a separate module so combat and quests remain compatible.
- Keep the original browser save key with backward-compatible settlement and terrain fields; this single-player game has no accounts or external database.
- Use deterministic world generation for the expanded biome network so saved terrain coordinates remain stable.
- Match the source game's indexed-access compiler behavior while keeping strict typing enabled; its fixed sprite palettes and tile arrays assume indexed values exist.
