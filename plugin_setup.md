# Setting up the plugins

By default, Project64 1.6 comes with Jabo plugins. While they generally work, they are ridden by many problems, such as missing shadows on Intel GPUs or crackly audio. This section provides information on recommended plugins as well how to set them up.

!!! Concerning manual setup
All the necessary plugins are already included with the provided Project64 build, but if you did the installation manually, you will have to install the plugins manually, too. This is typically done by copying the plugin .dll files, as well as any other files into the Plugin folder inside Project64's installation directory.
!!!

## Plugin selection

The plugins can be changed by opening the **Options -> Settings** menu. The **Plugins** tab should be selected by default.

### Graphics plugins
- **Recommended:** [**LINK's GLideN64**](gliden64_link.md)
- Alternatives: [GLideN64 rev.8004dc2](gliden64_old.md) or [glN64](gln64.md)

### Audio plugins
- **Recommended:** [**Azimer’s HLE v0.60 WIP 2**](azi60.md)
- Alternative: [shunyuan’s HLE audio](shunyuan.md)

### Controller plugins
Unfortunately there is a lot of controller plugins with their own set of quirks, and the optimal choice depends on the type of controller used.

- For **Raphnet N64 to USB v3** adapter: [**raphnetraw**](raphnetraw.md)
- For **Xbox**, **Dualshock 4/5**, **Switch Pro Controller** or other **XInput** controllers: [**Octomino's SDL Input**](octomino.md).
- For **keyboard**: [**LINK's DirectInput**](keyboardinput.md)
- For other DirectInput controllers: [**N-Rage's DirectInput**](nrage.md)