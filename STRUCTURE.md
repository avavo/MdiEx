# Repository structure

## `MdiEx_Nativo/`

Main clean package. This is the base version and includes NRAMV and LayerCache.

## `optional-drivers/`

Separated Vulkan driver files. These are not part of the clean native base unless a specific release needs them.

## `vortek-layer/`

Vortek Xclipse compatibility layer and its Vulkan manifest.

## `releases/`

Reference ZIPs. Prefer publishing release ZIPs through GitHub Releases instead of relying only on this folder.

## Root files

- `README.md`: main project explanation.
- `LICENSE`: project license for original files.
- `THIRD_PARTY_NOTICES.md`: ownership and license notes for included components.
- `RELEASE_NOTES_v3.0.md`: release summary.
- `CHECKSUMS_SHA256.txt`: integrity hashes.
