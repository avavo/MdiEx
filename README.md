# MdiEx

MdiEx is an experimental Vulkan compatibility layer package focused on Samsung Xclipse/Exynos devices.

This repository exposes the editable package structure directly instead of hiding everything inside a single ZIP. The ready-to-use ZIP can still be kept in GitHub Releases, but the repository itself should remain inspectable, forkable and easy to modify.

## What is included

```txt
MdiEx_Nativo/
├── libnramv.so
├── libVkLayer_Cache.so
├── meta.json
└── VkLayer_cache.json

optional-drivers/
├── vulkan.xclipse24.3.9.so
├── vulkan.xclipse2.0.0.so
└── vulkan.samsung.so

vortek-layer/
├── libVkLayer_VortekXclipse.so
└── VkLayer_vortek_xclipse.json

docs/
├── INSTALL.md
└── STRUCTURE.md

releases/
└── MdiEx_Nativo_v3.0.zip
```

## Core package

`MdiEx_Nativo` is the clean base package. It includes:

- `libnramv.so`, used for RAM pressure reduction and runtime memory handling.
- `libVkLayer_Cache.so`, the LayerCache Vulkan layer.
- `VkLayer_cache.json`, the Vulkan layer manifest.
- `meta.json`, the package metadata used by compatible loaders/emulators.

## Optional files

The files inside `optional-drivers/` and `vortek-layer/` are separated from the native package so users can clearly see what is core and what is optional.

## Recommended GitHub layout

Use this repository for exposed files, documentation and configuration. Put user-ready ZIPs under GitHub Releases.

Do not present a ZIP-only repository as fully open-source unless the actual editable source code is also exposed. A ZIP-only repo is technically visible, but socially it looks like a locked door with a window painted on it.

## Status

Version: v3.0  
Target: Samsung Exynos/Xclipse devices  
Minimum Android API: 34  
Package type: native MdiEx base package

## Disclaimer

This is an experimental compatibility package. It may break apps, games, emulators, Vulkan loading, or performance behavior depending on device, firmware, Android version and loader.

Use it for testing and development. Do not promise universal compatibility.
