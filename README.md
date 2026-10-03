# framebudget assets

Brand and launch video for [framebudget](https://framebudget.dev). The library lives in [framebudget/core](https://github.com/framebudget/core) and the website in [framebudget/website](https://github.com/framebudget/website).

## brand/

- `index.html`: the brand guide (logo, color, type, icons, motion, components). Open it in a browser.
- `logo/`: the mark, wordmark and lockups as SVG, the favicon, and PNG renders (`avatar-2048.png` for profile pictures, `mark-2048.png` on a transparent background).
- `fonts/`: Archivo, Martian Mono, Sixtyfour and Unbounded (SIL Open Font License 1.1, licenses next to each font).
- `tokens.css`, `tokens.json`: the color, type and spacing tokens.
- `og.png`: the social preview, rendered from `build/og.html` at 1200x630.
- `build/release.html`: the release card template. The release workflows of the library and the website check this repository out and render it with headless Chrome.

## video/

The launch video, a [HyperFrames](https://hyperframes.dev) project. `BRIEF.md` and `STORYBOARD.md` describe it; `npm run dev` previews it and `npm run render` renders `out/framebudget.mp4`.

The website copies what it needs (fonts, logos, `og.png`) into its own `docs/public/`; this repository is the source.
