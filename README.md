# Gaurav-Gosain/homebrew-tap

This is the Homebrew tap for my projects.

## Packages

| Name | Type | Install | What it is |
| --- | --- | --- | --- |
| [tuios](https://github.com/Gaurav-Gosain/tuios) | cask | `brew install gaurav-gosain/tap/tuios` | Terminal window manager |
| [tuios-web](https://github.com/Gaurav-Gosain/tuios) | cask | `brew install gaurav-gosain/tap/tuios-web` | Web terminal server for tuios |
| [golars](https://github.com/Gaurav-Gosain/golars) | formula | `brew install gaurav-gosain/tap/golars` | DataFrames for Go |
| [cider](https://github.com/Gaurav-Gosain/cider) | cask | `brew install gaurav-gosain/tap/cider` | Apple Foundation Models in Go. macOS on Apple silicon only. |
| [scraped](https://github.com/Gaurav-Gosain/scraped) | cask | `brew install gaurav-gosain/tap/scraped` | Scrapes web pages to Markdown |
| [streamd](https://github.com/Gaurav-Gosain/streamd) | cask | `brew install gaurav-gosain/tap/streamd` | Renders streamed LLM output as Markdown |

tuios is also in homebrew-core. `brew install tuios` installs the homebrew-core formula. The core formula and the `tuios` cask both install a `tuios` binary, so install only one of them.

## How the files change

GoReleaser writes every file in `Casks/` and `Formula/` when a project makes a release. A change made here is lost at the next release. To change a package, edit the `.goreleaser.yml` file in the project repository.

## Checks

The `checks` workflow runs `brew style` and `brew audit --cask` on each push to `main` and on each pull request. The workflow file lists the checks it skips and the reason for each.

## License

MIT. See [LICENSE](LICENSE).
