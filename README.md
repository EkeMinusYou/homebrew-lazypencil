# Homebrew tap for lazypencil

This tap distributes [lazypencil](https://github.com/EkeMinusYou/lazypencil), a
terminal-first `.pen` design editor, renderer, and MCP server.

## Install

The upstream signed release workflow populates `Casks/lazypencil.rb`. If that file
is not present yet, the first signed release has not completed. Once available:

```sh
brew install --cask ekeminusyou/lazypencil/lazypencil
brew upgrade --cask lazypencil
```

Supported releases require Apple Silicon and macOS 15.7.9 or later. Check the
upstream documentation for supported terminals and optional runtime setup.

## Maintenance

The upstream release workflow builds, signs with Developer ID, notarizes, verifies,
and publishes the complete binary package before updating this tap. Versions and
SHA-256 checksums are generated from that verified archive. Do not edit the Cask by
hand or replace published release assets.

The complete package stays in Homebrew's Caskroom, including corresponding source,
original third-party notices, and build evidence. The executable is linked onto
`PATH`. Upstream setup and credential requirements are documented in the
[development guide](https://github.com/EkeMinusYou/lazypencil/blob/main/docs/development.md#signed-releases-and-the-dedicated-homebrew-tap).
