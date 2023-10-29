# 1. Windows/Driver/Software

When it comes to Windows, bet to use a clean, not trimmed Version of Windows 11 in your Language.
Trimmed Versions like Tiny11 brings more issues than its worth.

ISOs can be found here:
https://massgrave.dev/msdl/

Or if you are the more Paranoid Type, can by build yourself from all the newest packages with UUPDump:
https://uup.ee/

Flash the Resulting ISO with RUFUS (https://rufus.ie/) to an USB Drive and Install it

Boot/BIOS Menu can be accessed by holding the Turbo Button on Boot. 

After Installing Windows install the Following Drivers in this specific Order:
1. OneXPlayer 2 Pro Official Driver Pack: 
https://onenetbook.oss-cn-beijing.aliyuncs.com/OnexPlayer/oxp2/OnexPlayer2Pro_EVA.rar
2. AMD Chipset Driver:
https://www.amd.com/en/support/chipsets/socket-fp5-mobile/amd-ryzen-and-athlon-mobile-chipset
3. AMD GPU Driver:
https://www.amd.com/en/support/apu/amd-ryzen-processors/amd-ryzen-7-processors-radeon-graphics/amd-ryzen-7-7840u
4. SDCard Reader:
https://www.intel.com/content/www/us/en/download/19604/genesys-sd-card-reader-driver-for-windows-10-64-bit-windows-11-for-intel-nuc-10-performance-kits-mini-pcs-nuc10ixfn.html
5. Generic Realtek Audio Driver:
https://github.com/pal1000/Realtek-UAD-generic/releases

Once all of that is installed, do a Reboot. Now we install the Device Control Panel. OneXplayer usually comes with OneXPanel. The Issue with that is that its bad. For that reason, we use HandheldCompanion.
It brings everything we need. Gyro, TDP, Performance Overlay, Controller Rebinding. Game Profiles, Resolution and Refresh rate switching, FPS Limiting and much more. It also has an excellent Controller Desktop Mode.

Download it from here and install it:
https://github.com/Valkirie/HandheldCompanion

### Additional things to consider
1. Turn off Windows Defender. (Won't tell you how, If you can't figure it out you probably should not.)
2. Turn off SmartScreen.
3. Delay Steam Autostart to make sure Handheld Companion is started first. Also make it run as Admin.
For that, Disable Steams Build in Autostart and create a scheduled task that runs at Logon with a delay of 30 Seconds. Also set the Tick to run with Highest Privileges.
4. Disable UAC.

# Display Resolution and Refreshrates

I modified the EDID of the Display to provide more Refreshrates and Resolutions to play with.
Especially more granular Refresh Rates help greatly with smoothness at lower Framerate.

[EDID .bin File](https://github.com/NightHammer1000/OneXPlayer2Pro_Tweaks/raw/main/OXP2P_Res_Refresh_Extended.bin)

[EDID Installer](https://github.com/NightHammer1000/OneXPlayer2Pro_Tweaks/raw/main/OXP2P_Res_Refresh_Extended.exe)

Import the EDID bin file in CRU or just run the Installer and Reboot.
Now you should have more options.

![Resolutions](https://i.imgur.com/26PgDYf.png)
![Refreshrates](https://i.imgur.com/HbRwa5Z.png)
 
# Must Have Software
## Lossless Scaling
AMD RSR is broken on the OneXplayer 2 Pro because it uses a Display which Refreshrates are Portrait Mode by Default. That breaks the Native Resolution Detection of RSR and the Upscaling never starts when you Drop below native Resolution.

But for every Issue there is a Solution. For this Problem we can use Lossless Scaling. 
This Software brings great Quality while Upscaling form Lower Resolutions.
The only Downside it has is that your Game has to run in Windowed Mode. Which can be a bit of a Pain with older Games, but for almost every Game [PCGamingWiki](https://www.pcgamingwiki.com/wiki/Home) can offer a solution.
Lossless Scaling can be bought here:
https://store.steampowered.com/app/993090/Lossless_Scaling/

### Setup and Integration
Buy it, Install It, Run it.
Set it to start on Boot, to minimize on Start and to close to Taskbar.
Set the Scaling Mode to LS1, tick Performance Mode.
Adjust Sharpness to your liking.

Now open Handheld Companion and edit the Controller Profile for the Default Profile.
Find the OEM Button. Add an Action. Set it to Long Press. Set the Key it sends to Z
Open the Advanced Settings. Set Modifier to Control + Alt

Now if you start a Game in Windowed Mode and long Press the Turbo Button you Upscale the Game to Full screen.
## USB Safely Remove
A small tool for the Info Area to Safely Unmount SD Cards for Swapping.
https://safelyremove.com/index.htm
## Steam-Library-Manager
SD Card performance under Windows is... well shit. Especially if you Install Games on it with Steam Directly. It WILL take ages.
Best to Download them to SSD and then use Steam-Library-Manager to move them over to SD Card.
https://github.com/RevoLand/Steam-Library-Manager
## Playnite
Hands down the best Fullscreen Launcher to combine all your Games from EPIC, GOG, XBOX, STEAM and many more in one Place.
They even Support Emulation Setups.
And best of all. Its Free.
https://playnite.link/
