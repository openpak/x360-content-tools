# OpenPak integration

This is OpenPak's fork of [Velocity](https://github.com/hetelek/Velocity).
The upstream GPL license and notices are preserved. OpenPak changes use `main`.

The first intended use is validating homebrew packages for the stock Xbox 360
HDD library and native Store installation flow. STFS/SVOD, title metadata,
package thumbnails and XDBF/profile inspection are relevant capabilities.

Initial integration work:

- Verify package output against Wharf's reader and a physical 17559 console.
- Make reproducible package-generation and inspection commands suitable for
  the OpenPak catalog pipeline, retaining package provenance and hashes.
- Test install, enumerate, launch, update and uninstall with one redistributable
  Xbox 360 homebrew title before expanding the catalog.

Creating a container does not establish executable trust or a working native
Store purchase/download flow. Those are separate integration requirements.
The fork has not yet been built or qualified for OpenPak packages.
