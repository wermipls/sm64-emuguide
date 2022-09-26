---
description: "Comprehensive emulator setup guide for Super Mario 64 speedruns"
---

# LINK's GLideN64

![](./img/gliden64_link.png)

[!file Download (manual setup only)](https://www.mediafire.com/file/k9ad2bdodde327u/GLideN64-sm64hacks.zip/file)

[!file Download (ANGLE DX11/Vulkan Edition)](https://www.mediafire.com/file/31n8khvmwx0ws73/GLideN64-angle.zip/file)

Arguably the best HLE graphics plugin available. This is a fork based on GLideN64 4.0, introducing some regressions that improve romhack compatibility. This version of the plugin also allows for aspect ratio correction with framebuffer disabled. 720p resolution is recommended to avoid framebuffer artifacts.

If ANGLE edition is used, make sure libEGL.dll and libGLESv2.dll are placed near the Project64.exe.

!!!warning
Make sure to **disable** framebuffer emulation, since it increases latency.
!!!

!!!warning
If using OBS, make sure to use the **Game Capture** source.
!!!

[!ref Return to plugin selection](plugin_setup.md#plugin-selection)
