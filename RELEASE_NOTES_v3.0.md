# MdiEx v3.0 Release Notes

MdiEx v3.0 is a native base package for Samsung Exynos/Xclipse devices.

## Included in the native package

- LayerCache v9 Vulkan layer.
- NRAMV runtime library.
- Vulkan layer manifest for LayerCache.
- Metadata file for compatible loaders/emulators.

## Purpose

This version is intended to provide a clean base for Vulkan compatibility testing, memory pressure reduction and package-level experimentation on Exynos/Xclipse devices.

## Notes

- `MdiEx_Nativo/` is the main package.
- `optional-drivers/` contains separated driver files.
- `vortek-layer/` contains the Vortek Xclipse wrapper layer and manifest.
- Ready-to-use ZIPs should be published in GitHub Releases.
