---
description: "Comprehensive emulator setup guide for Super Mario 64 speedruns"
---

# ANGLE GLideN64 (LINK's GLideN64)

![](./img/gliden64_link.png)

[!ref target="blank" text="Download"](https://github.com/aglab2/GLideN64/releases)
[!file Download (old version)](https://www.mediafire.com/file/k9ad2bdodde327u/GLideN64-sm64hacks.zip/file)

Arguably the best HLE graphics plugin available. This is a fork of GLideN64, introducing some regressions that improve romhack compatibility. This version of the plugin also allows for aspect ratio correction with framebuffer disabled. 720p resolution is recommended to avoid framebuffer artifacts. The ANGLE version also introduces DX11 and Vulkan backends, while still keeping the legacy OpenGL backend as an option.

!!!warning
Make sure to **disable** framebuffer emulation, since it increases latency.
!!!

!!!warning
If using OBS, make sure to use the **Game Capture** source.
!!!

[!ref Return to plugin selection](plugin_setup.md#plugin-selection)
