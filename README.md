# homebrew-tap

Homebrew tap for [webpage2pdf](https://github.com/Nornchan/webpage2pdf) —
turns web pages into clean A4 PDFs that read like typeset essays.

## Install

```bash
brew install Nornchan/tap/webpage2pdf
```

That puts three commands on your `PATH`: `webpage2pdf`, the shorter alias
`w2p`, and `webpage2pdf-server` (a local drag-and-drop web app).

## Changelog

### [v0.1.1](https://github.com/Nornchan/webpage2pdf/releases/tag/v0.1.1) — 2026-09-07

Homebrew packaging fix — the formula did not actually build from source.
`cmake`, `ninja` and `pkg-config` were missing as build-time dependencies,
which broke Pillow's build inside Homebrew's sandboxed build environment.
Fixed and verified with `brew install` from a genuinely fresh, untapped,
untrusted machine state, and `brew upgrade` from a real 0.1.0 install.
If you installed 0.1.0, `brew upgrade webpage2pdf` picks this up.

### [v0.1.0](https://github.com/Nornchan/webpage2pdf/releases/tag/v0.1.0) — 2026-09-07

First packaged release.

Full notes for every version are in
[`packaging/RELEASE.md`](https://github.com/Nornchan/webpage2pdf/blob/main/packaging/RELEASE.md#changelog)
in the main repository.

## Updating the formula

The formula lives in [`Formula/webpage2pdf.rb`](Formula/webpage2pdf.rb) and is
kept in sync with [`packaging/webpage2pdf.rb`](https://github.com/Nornchan/webpage2pdf/blob/main/packaging/webpage2pdf.rb)
in the main repository, which is where changes should be made first.
