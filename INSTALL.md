# Installation notes

This repository is organized for GitHub visibility and modification.

For normal users:

1. Download the ready-to-use ZIP from Releases.
2. Import or place it where your emulator/loader expects driver packages.
3. Keep the internal structure intact.

For contributors:

1. Inspect `MdiEx_Nativo/` first.
2. Modify manifests or metadata only if you understand the target loader.
3. Keep optional driver files separated unless a specific release requires them.
4. Rebuild a release ZIP only after testing the package structure.

## Important

Do not mix every `.so` file into the native package root unless the loader expects that exact layout. Randomly throwing binaries into a folder is not engineering, it is confetti with consequences.
