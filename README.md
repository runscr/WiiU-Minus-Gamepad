# WiiU-Minus-Gamepad
Documentation on using a Wii U without a Gamepad


## Wii U Initial Setup without Gamepad
Directions:
- Install isfshax or a de_fuse modchip, with minute running from coldboot
- If you need to rebuild your MLC (corruption issues, etc) do it at this point.
  - Make sure to remove wafel_setup_mlc.ipx from `sd:/wiiu/ios_plugins` after rebuild is complete
  - Boot with patches to verify that the MLC is functioning correctly
  - Shutdown Wii U and remove SD card
- Copy 'wafel_payloader.ipx' to `sd:/wiiu/ios_plugin`
- Copy Aroma CFW to SD card. [Click here for an SD preparation guide](https://wiiu.hacks.guide/aroma/sd-preparation.html) 
- Download the 'Better SysApps' plugin from the following link: [Better-SysApps](https://github.com/runscr/Better-SysApps/releases))
- Copy 'BetterSysApps.wps' to `sd:/wiiu/environments/aroma/plugins`
- Download the modified recovery menu from here: [recovery_menu_init-launch-1](https://github.com/runscr/WiiU-Minus-Gamepad/releases/tag/recovery-menu)
- Copy 'recovery_menu_init-launch-1' to `sd:/recovery_menu`
- Reboot console, use the [UDPIH exploit](https://github.com/GaryOderNichts/udpih) to load the recovery menu
- Navigate to the 'Set Initial Launch Value' menu
- Select the following initial launch value: `1 - Initial Account Setup`
- Reboot the console
- The initial account creation screen should appear.
- Press the sync button *twice* on your Wii U and sync a compatible controller.
- Navigate through the setup, eventually you will land at the Wii U menu.
- Open 'System Settings' and configure the following items:
  - Date and Time
  - TV display settings
  - Power Settings
    - Disable Standby (if you would like)
  - Console Information
    - Set System Language
    - Set Country of Residence
- Exit out of settings and you're done!
