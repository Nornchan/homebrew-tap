# homebrew-tap

Homebrew tap for [webpage2pdf](https://github.com/Nornchan/webpage2pdf) —
turns web pages into clean A4 PDFs that read like typeset essays.

## Install

```bash
brew install Nornchan/tap/webpage2pdf
```

That puts three commands on your `PATH`: `webpage2pdf`, the shorter alias
`w2p`, and `webpage2pdf-server` (a local drag-and-drop web app).

## Updating the formula

The formula lives in [`Formula/webpage2pdf.rb`](Formula/webpage2pdf.rb) and is
kept in sync with [`packaging/webpage2pdf.rb`](https://github.com/Nornchan/webpage2pdf/blob/main/packaging/webpage2pdf.rb)
in the main repository, which is where changes should be made first.
