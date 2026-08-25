# homebrew-tap

Homebrew formulae for [nexdrew](https://github.com/nexdrew) tools.

```sh
brew install nexdrew/tap/blitzy-cli   # standalone `blitzy` binary, no Node required
```

Formulae here are machine-generated: `Formula/blitzy-cli.rb` is rendered from each
release's asset digests by the [blitzy-cli release workflow](https://github.com/nexdrew/blitzy-cli/blob/main/.github/workflows/release.yml)
(`scripts/homebrew-formula.mjs` is the source of truth). Don't edit formulae by hand —
changes belong in the generator.

Every binary the formulae install carries a GitHub build-provenance attestation:

```sh
gh attestation verify "$(command -v blitzy)" --repo nexdrew/blitzy-cli
```

(`command -v blitzy` resolves the brew symlink to the installed binary, and — unlike
`$(brew --prefix)/bin/blitzy` — it works on machines with more than one Homebrew
prefix, e.g. an Intel brew at `/usr/local` alongside `/opt/homebrew`.)
