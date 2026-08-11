# GRU953-Studio Homebrew tap

[![formula](https://img.shields.io/badge/dynamic/regex?url=https%3A%2F%2Fraw.githubusercontent.com%2FGRU-953%2Fhomebrew-tap%2Fmain%2FFormula%2Fgru953-studio.rb&search=studio-cli-%28%5B0-9.%5D%2B%29.tgz&replace=v%241&label=formula&color=00AE99)](Formula/gru953-studio.rb)
[![licence](https://img.shields.io/badge/licence-PolyForm%20Noncommercial%201.0.0-B28400)](https://github.com/GRU-953/GRU953-Studio/blob/main/LICENSE)
[![GRU953-Studio](https://img.shields.io/badge/GRU953--Studio-repository-3257A0)](https://github.com/GRU-953/GRU953-Studio)

The Homebrew formula for the [GRU953-Studio](https://github.com/GRU-953/GRU953-Studio)
command, for macOS and Linux.

<sub>The version above is read live from the formula in this repository, so it cannot
drift out of date. Homebrew's own shields.io badge only covers formulae in Homebrew
core, not taps, which is why this one reads the file directly.</sub>

## Install

```
brew install GRU-953/tap/gru953-studio
```

**Homebrew 6 may ask you to trust this tap first.** Homebrew now refuses to load a
formula from a third-party tap until you say you trust it — a sensible precaution,
since a tap is just somebody's repository. If you see a message about an
"untrusted tap", run this once and then install again:

```
brew trust GRU-953/tap
```

If you are never asked, you have nothing to do — the install simply proceeds.

Then, when you are ready:

```
gru953-studio install
```

That looks for Claude Code, Claude Desktop, Google Antigravity, VS Code, Cursor and
Windsurf on your computer and sets the studio up in each one it finds. It asks
before changing anything.

Installing the formula deliberately does **not** run that step for you: it writes
into your editors' configuration, which is not something a package manager should
do without being asked.

## Other ways to install

This tap is one of several routes, and you only need one:

| Route | Best when |
| :-- | :-- |
| **This tap** | You are on macOS or Linux and install things with Homebrew |
| `npm install -g @gru953/studio-cli` | You already have Node.js |
| The one-line installer | You want everything set up in a single paste — see the [main README](https://github.com/GRU-953/GRU953-Studio#quick-start-one-time-setup) |
| A downloadable installer per app | You prefer a file — see [Releases](https://github.com/GRU-953/GRU953-Studio/releases) |
| Inside Claude Code | `/plugin marketplace add GRU-953/GRU953-Studio` |

## Why a tap rather than Homebrew core

Homebrew's main catalogue applies notability criteria that are Homebrew's own
maintainers' to judge, not something this project can assume. A tap is entirely
within this project's control and works immediately, so that is what this is.

## Keeping it current

The formula's `url` and `sha256` point at one specific published version. When a
new GRU953-Studio version is released, both lines are updated here. To get the
newest:

```
brew update && brew upgrade gru953-studio
```

## Licence

GRU953-Studio is free for non-commercial use under the
[PolyForm Noncommercial License 1.0.0](https://github.com/GRU-953/GRU953-Studio/blob/main/LICENSE).
Selling something built with it needs a separate licence — see
[COMMERCIAL-LICENCE.md](https://github.com/GRU-953/GRU953-Studio/blob/main/COMMERCIAL-LICENCE.md).

This tap contains only packaging metadata; the software itself lives in the
[main repository](https://github.com/GRU-953/GRU953-Studio).
