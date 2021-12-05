## Picking a controller

If you haven't decided what to play on, or are considering what to buy, below is a list of some of the common options, subjectively ordered from best to worst. For detailed setup instructions, refer to the **Setting up the controller** section below.

 - **Original Nintendo 64 controller with [raphnet 3rd generation N64 to USB adapter](https://www.raphnet.net/electronique/gcn64_usb_adapter_gen3/index_en.php)** - this is about as close as it gets to console experience. Very low latency and raw input plugin available for 100% input mapping accuracy amongst other things. Somewhat pricey if buying from raphnet's store, but you can also [make your own for cheap](https://wermi.neocities.org/posts/raphnet-diy/). **Note on other generic adapters** - those will often have issues such as inability to press all four C buttons at once, not functioning correctly with Hori Minipad or poor pollrate/latency (especially avoid the old dual port Mayflash). Buy at your own risk.
 - **Nintendo Gamecube controller with official Wii U USB adapter** - decent controller option, requires drivers to function. Mayflash clone of the adapter (set to Wii U mode) also works fine with the drivers. Other generic clones may have issues, but should work in PC mode. If you don't mind the price, you may want to buy raphnet GC to USB for driverless experience.
 - **Xbox 360 or Xbox One controllers** - another solid choice, although the lack of notches can hinder the gameplay. Unfortunately most controller plugins seem to have issues with those, as well as other XInput controllers.
 - **Nintendo Switch Pro Controller** - roughly on par with Xbox, but requires drivers to function. 
 - **Sony Dualshock 3/4** - roughly on par with above. Drivers for Dualshock 3 are not maintained anymore.
 - **Keyboard** - yes, you can play this game on keyboard. Although not optimal, it has been  [proven to not be a hindrance at least until top level](https://www.twitch.tv/videos/546951097).

## Setting up the controller
This section will mostly outline where to get drivers and which plugins to use with each controller. More detailed information on usage of each plugin can be found in the **Setting up the plugins** section.

### N64 with raphnet v3 adapter
There are two ways to use the adapter: either using the raphnetraw plugin, or through DirectInput using the N-Rage input plugin. While the former provides 100% accurate inputs to console, the latter allows to do things not normally possible with raphnetraw, such as setting up custom macros or switching controllers for throws.

#### Raw input via raphnetraw plugin
[Download the plugin from here](https://www.raphnet.net/programmation/mupen64plus-input-raphnetraw/pj64raphnetraw-1.0.6.zip). Copy **libhidapi-0.dll** to your **Project64 installation folder**, and all the remaining .dll files to the **Plugin** folder. Go to **Options -> Settings**, select the raphnetraw plugin and you are done. 

#### N-Rage input plugin 
Use **N-Rage 1.83** or **2.3c**, see details in **Setting up the plugins** section below. Make sure to set **deadzone** to **0%**, uncheck **Real N64 Range** and adjust the range slider so the values you get are as close as possible to what you'd get on raphnetraw.

### Gamecube controller with Wii U adapter
[Go to Massive's website](http://m4sv.com/page/wii-u-gcn-usb-driver), download the drivers and follow the instructions on the page. If using a 3rd party adapter, make sure to set it to Wii U mode. After installing the drivers, use **N-Rage 1.83** plugin (see details in **Setting up the plugins** section), make sure to select **vJoy device** in the **Devices** tab and uncheck **Real N64 Range**. GiBoss has made a config file with preconfigured binds, which you can get [here](https://drive.google.com/file/d/0B6VO6sgQUsMVclR2enpZc29BYUU/view?usp=sharing). If your controller is not getting recognized, try using **N-Rage 2.3c** instead.

### Xbox controller
Use **Billard's XInput** plugin. No configuration, copy the .dll to the **Plugin** folder and you are done. If you want to set your own binds, you will have to use **N-Rage**, which tends to have issues with XInput controllers. See details in **Setting up the plugins** section.

### Switch Pro Controller
I strongly recommend using [BetterJoy](https://github.com/Davidobot/BetterJoy) for drivers. Follow the instructions on the page. After that, refer to **Xbox controller** section above for the plugins.

### Dualshock 4
I suggest using [Ryochan's fork of DS4Windows](https://ryochan7.github.io/ds4windows-site/) for drivers. Follow the instructions on the page. After that, refer to **Xbox controller** section above for the plugins.

### Dualshock 3
Although unmaintained, [ScpToolkit](https://github.com/nefarius/ScpToolkit/releases) still seems to be the best solution for DS3 drivers. Refer to **Xbox controller** section above for the plugins.

### Other/generic controllers
Use N-Rage if it's a DirectInput controller or Billard for XInput controllers. See details in **Setting up the plugins** section.

### Keyboard
Use [LINK's DirectInput plugin](https://cdn.discordapp.com/attachments/329337636244291587/421198571266768907/KeyboardInput.zip). This is a modification of Jabo's DirectInput meant for keyboard players, which adds support for analog modifiers (so you can e.g. walk instead of running). The modifiers are configured through the **KeyboardInputConfig.txt** file, which specifies the **amount by which the analog values get divided** next to **virtual-key codes**, which specify the buttons triggering the modifiers. A full list of those key codes can be found [here](https://docs.microsoft.com/en-gb/windows/win32/inputdev/virtual-key-codes). For example, the first line of the default config file is `2 4C`, which means the analog value will get halved when the L key is held. The plugin will only read 5 lines of the config, so you will probably have to delete the existing binds.

## Setting up the plugins


### Controller plugins

#### Billard's XInput
A simple plugin with rumble support. No configuration needed (or possible). Download here.

If you get an error loading the plugin, install [DirectX End-User Runtime](https://www.microsoft.com/en-US/download/details.aspx?id=35).

### Graphics plugins

### Audio plugins 
