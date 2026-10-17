# wow-optimize-ci

Manual GitHub Actions build of [suprepupre/wow-optimize](https://github.com/suprepupre/wow-optimize)
from any branch, tag or commit, for trying unreleased changes.

- Runs the project's own `build.bat` on `windows-2025-vs2026` (MSVC, Win32,
  Release), the toolchain the official releases use.
- Run: `gh workflow run build.yml --repo mybaixinyu/wow-optimize-ci -f ref=main`
- Artifact `wow-optimize-build`: `wow_optimize.dll`, `wow_optimize.sym`,
  `version.dll`, the launcher, and `BUILD-INFO.txt` (commit and hashes).
