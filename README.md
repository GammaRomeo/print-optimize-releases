# print-optimize-releases

Public version pointer for [Print Queue Optimizer](https://github.com/GammaRomeo/Print-Optimize)
self-hosted installs.

This repo intentionally contains **no source code, configuration, or
credentials** -- only plain-text version files. Each installed copy of the
app (and its optional Klipper companion agent) periodically checks the
relevant file's contents (a simple unauthenticated HTTPS GET, since this
repo is public) against its own local version, and shows an in-app notice
if a newer version has been released.

- `VERSION` -- the main app.
- `COMPANION_VERSION` -- the Klipper companion agent (`klipper_companion/`
  in the main repo), versioned independently since it changes on a much
  slower cadence.

The main application repository is private; this repo exists solely so
external installs have something to check without needing access to it.

## Releasing a new version

Bump the version number in the relevant file (`VERSION` or
`COMPANION_VERSION`) and commit it, once the corresponding release is
actually out. That's the entire release process from this repo's side.
