# Fonts

Apple's **SF Mono** family, extracted from `Terminal.app`
(`/System/Applications/Utilities/Terminal.app/Contents/Resources/Fonts`),
plus **Dank Mono** patched with [Nerd Font](https://www.nerdfonts.com) glyphs.

| Files | Family name | Used by |
|---|---|---|
| `SF-Mono-*.otf` (Light → Heavy + italics) | `SF Mono` | zed, vscode |
| `SFMono-Terminal.ttf`, `SFMonoItalic-Terminal.ttf` | `SF Mono Terminal` | ghostty (`font-family = SF Mono Terminal`) |
| `DankMonoNerdFont-*.otf` (Regular, Bold, Italic) | `DankMono Nerd Font` | — icons keep their natural width |
| `DankMonoNerdFontMono-*.otf` (Regular, Bold, Italic) | `DankMono Nerd Font Mono` | — icons forced to one cell; prefer this in terminals |

## Install

```sh
cp *.otf *.ttf ~/Library/Fonts/
```
