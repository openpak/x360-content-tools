# Deploy: x360-content-tools

## Build

Prerequisites (see [COMPILING.md](../COMPILING.md) for per-platform steps):

- Qt 6 (`qmake` on the PATH).
- Botan 3.4. `.gitmodules` declares a `botan` submodule, but it is not checked out in this tree, so Botan must come from the system or a local install.

Makefile targets:

- `make debug` builds the debug configuration. Running `make` with no target is the same as `make debug`.
- `make release` builds the release configuration.
- `make clean` removes the build outputs.

The Makefile builds `XboxInternals` first (copied to `XboxInternals-<OS>/<CONFIG>`), then `Velocity`.

Platform scripts:

- `build_mac` runs `qmake6`, `make`, `macdeployqt6` and `codesign`. The signing identity is the placeholder `DEVELOPER_ID_HERE` and must be replaced before use.
- `build_windows.ps1` is the Windows build script.
