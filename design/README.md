# Profile artwork source

`profile.html` is the editable source for the GitHub profile artwork. It uses the portfolio's white background, `#1263e8` accent, Pretendard typeface, and actual published project screenshots.

The published README uses six separately linked image panels. Each panel has a desktop and a mobile export in `assets/profile-v2/`. Mobile variants use a stacked layout to keep their text readable. No JavaScript, remote font server, or external image service is needed when viewing the profile.

## Rendering

Serve the repository root with a local static HTTP server and open `design/profile.html` in Chromium. Wait for `document.fonts.ready` and all images to load. Capture each `[data-asset]` element independently, preserving the white background and padding. Desktop exports use a 971 CSS-pixel viewport; mobile exports use 344 CSS pixels. Both use a device scale factor of 2.

Panel order: `hero`, `economics`, `sleep`, `oil`, `plushome`, `footer`.

The HTML preview contains real links. In GitHub's README, the enclosing link covers the whole corresponding image, including the visually indicated action. Source-code links and selectable text descriptions are also provided below the artwork in an expandable section.

## Sources and notices

- Project screenshots: existing public `polalise.github.io/media/projects/*/cover-960w.webp` assets, copied without changing their pixels. The source layout frames them with CSS.
- Pretendard Variable: [orioncactus/pretendard](https://github.com/orioncactus/pretendard). License and copyright notice: `fonts/Pretendard-LICENSE.txt`.
- IBM Plex Mono: [IBM/plex](https://github.com/IBM/plex). License and copyright notice: `fonts/IBMPlexMono-LICENSE.txt`.
- GitHub mark: [Simple Icons](https://github.com/simple-icons/simple-icons/blob/develop/icons/github.svg), CC0. Brand marks remain the property of their respective owners.

The design matches the approved concept's content and hierarchy. The project images are the original screenshots rather than the text and graphics reconstructed by the concept image generator.
