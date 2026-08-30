# print-optimize-releases

Public version pointer for [Print Queue Optimizer](https://github.com/GammaRomeo/Print-Optimize)
self-hosted installs.

This repo intentionally contains **no source code, configuration, or
credentials** -- only a plain-text `VERSION` file. Each installed copy of
the app periodically checks this file's contents (a simple unauthenticated
HTTPS GET, since this repo is public) against its own local version, and
shows an in-app notice if a newer version has been released.

The main application repository is private; this repo exists solely so
external installs have something to check without needing access to it.

## Releasing a new version

Bump the version number in this file's `VERSION` (and commit it) whenever
a new version of the app is released. That's the entire release process
from this repo's side.
