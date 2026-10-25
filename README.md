# Xbox 360 Content Tools

OpenPak's Xbox 360 Content Tools.

| | |
| --- | --- |
| Console | Xbox 360 |
| Kind | Desktop app (Qt 6) with the `XboxInternals` library |
| Based on | [Velocity](https://github.com/hetelek/Velocity) (GPL-3.0-or-later, as upstream) |

## What it does

- Browses and edits Xbox 360 files: STFS, SVOD, GDFX, FATX, XDBF, YTGR, Xbox-specific cryptography, and the Account file.
- The file-format backend is the `XboxInternals` library in `XboxInternals/`.

## Build

```sh
make release
```

Needs Qt 6 and Botan 3.4. See [deploy](docs/deploy.md).

## Docs

- [Protocol](docs/protocol.md)
- [Evidence](docs/evidence.md)
- [Deploy](docs/deploy.md)
- [Notes](docs/notes.md)
- [Upstream README](docs/upstream.md)
