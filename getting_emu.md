---
description: "Comprehensive emulator setup guide for Super Mario 64 speedruns"
---

# Acquiring the emulator

The only version of Project64 allowed on the leaderboards is 1.6. **All other versions (such as 1.7 or 2.x) are banned.** The leaderboards also permit usage of Mupen64Plus and OpenEmu, providing native emulation options for Linux and Mac users respectively. This guide focuses on setting up Project64 1.6 specifically. 

## Download

To speed up the configuration process, there's a prebuilt package available with the emulator and the best plugins. Extract the archive into any location you want, then follow the next sections in the guide.

!!!
If you get errors while loading any of the plugins, you will have to install the appropriate Visual C++ runtimes. For convenience, an all-in-one package can be found here: https://www.techpowerup.com/download/visual-c-redistributable-runtime-package-all-in-one/
!!!

[!file Mirror 1 (Dropbox)](https://www.dropbox.com/s/ku6eyhkubot000r/Project64%201.6%20%28wermi%27s%20build%20v2%29.zip?dl=1)
[!ref target="blank" text="Mirror 2 (GDrive)"](https://drive.google.com/file/d/1N5GCsCE-MhrXTZym5CDoPUMb7ehwAr0u)

Last updated on 2021-05-10.

## Manual setup

!!!warning

The guide is written with the assumption that you are using the build provided above to streamline the process. Manual install is possible, but not really recommended. I'm not your mom, though :shrug:

!!!

If you want to set up the emulator manually, you can also [download Project64 1.6 directly from Jabosoft](http://www.jabosoft.com/articles/114), along with a patch updating the default Jabo plugins for better compatibility. Run the 1.6 installer first, then apply the 1.6.1 patch by either running the installer or by copying the plugins to the Plugin folder in case of the .zip version. 

!!!

It is suggested the emulator is installed **somewhere else than Program Files**, for example `C:\Project64 1.6`. This is because write permissions are restricted for that directory in newer versions of Windows, and any writes performed by legacy applications will get redirected to a VirtualStore folder, causing you to wonder e.g. where your save files exactly are.

!!!
