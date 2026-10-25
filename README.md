# ashtonian/tap

Homebrew casks for [ashtonian](https://github.com/ashtonian)'s tools.

| Cask | What it is |
| --- | --- |
| [gitstead](https://github.com/ashtonian/gitstead) | Find, clone and keep in sync every repo you work on across GitHub, GitLab and Gitea/Forgejo, then launch coding agents on them side by side. |

## Install

```bash
brew install --cask ashtonian/tap/gitstead
```

Name the cask in full, `ashtonian/tap/<cask>`: Homebrew requires trust for
taps outside its own, and installing by the full name trusts that cask, so
`brew upgrade` keeps it current. To use short names, or every cask here, trust
the whole tap with `brew trust --tap ashtonian/tap`.

Existing installations should follow the [migration instructions](https://github.com/ashtonian/gitstead/releases/tag/v0.3.0) before upgrading.

## Notes

- The binaries aren't notarized by Apple. Homebrew quarantines what it
  downloads, so each cask clears the quarantine on the binary it installs;
  without that, macOS would refuse to run it.
- Each cask has macOS and Linux builds, for Intel and ARM.
- Casks are written by each tool's release (GoReleaser); don't edit them by
  hand. Report problems with a tool in that tool's repository.

## Uninstall

```bash
brew uninstall --cask gitstead
```

Some tools install things of their own, such as a background schedule; the
cask's caveats (`brew info --cask <cask>`) say what to remove first.
