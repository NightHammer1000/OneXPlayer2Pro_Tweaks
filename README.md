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
