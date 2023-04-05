
This is just a mirror of my Hyprland-dots I used for youtube. Link below


https://github.com/JaKooLit/Ja_HyprLanD-dots

## ✨ Arch Linux quick Installation:

A guide to install :[`Youtube Link`](https://youtu.be/_deaeSU1WK8)

1.) optional: you can install nvidia-all driver from Frogging Family to replace the nvidia-drivers 
 - chmod +x nvidia-all-driver and run with nvidia-all-driver

a.) Install yay (chmod +x yay-bin-install and run the script). You can also install paru if desired

b.) You can install one by one packages or choose the automatic installer script. (chmod +x install-hyprland and run the script). 
NOTE. If you install paru instead of yay, ensure to edit install-hyprland and change all yay with paru

c.) If you want to add or edit packages, edit install-hyprland script. Check first if packages are present on AUR or official else the script will fail.

d.) Installation of Asus-ROG-utilities are entirely optional. if you select no, will skip the step.



## ✨ Manual Installation and Notes: 
### you can copy, create, change, however, would appreciate if you have have a better solution / changes so we will all improve :)

These configs are used in my Laptop and Desktop. 
Please note, Only provided are configs. Any Hyprland-related issues to be reported on Hyprland Github

a.) Copy / Move files / folders in your ~/.config

b.) Put wallpapers in your ~/Pictures/

c.) if you want in Arch, make sure to comment / uncomment some items in /hypr/configs/exec.conf - location of polkit is different than gentoo, By default, all configs are set to work with Arch Linux

d.) If you use `thunar` as file manager, suggested additions for thunar (thunar-volman, tumbler, gvfs, gvfs-mtp (for accessing phone), Thunar archive plugin-ins) See Arch wiki https://wiki.archlinux.org/title/thunar

e.) make sure scripts located at /hypr/scripts/ are executable as required. (use chmod +x or right click, properties, change permission to be executable)

f.) Inspect /hypr/configs/exec.conf Choose which polkit gnome to use. to use. (Gentoo have different location of executables. Arch /usr/lib vs Gentoo /usr/libexec) Polkits by default are set to Arch Linux

g.) if you have azerty keyboard [`this`](https://github.com/swaywm/sway/issues/1460?fbclid=IwAR1C8VcY_wWbGhXvT-5ApjJCQuJoJzhOVor6o5fdn0Nj1c6bD9JXoQAPQIg) might help



## ✨ Gentoo Specific notes

<details>
<summary>
Gentoo Specific
</summary>

1. [`Hyprland - Link to zugaina`](https://gpo.zugaina.org/gui-wm/hyprland) have 3 overlays. I am using wayland-desktop overlay. Nvidia and openrc users, you should look into thegreatmcpain overlay. Or of course you can compile hyprland from source
2. Waybar - from Gentoo repo's waybar, I experienced unclickable workspaces. I have installed from useless-overlay. Click [`here`](https://github.com/JaKooLit/Ja_HyprLanD-dots/blob/main/misc/Gentoo-Waybar) for guidance
3. For screen sharing, I use xdg-desktop-portal-wlr which seems to work. If you are having issues, install xdg-desktop-portal-hyprland
4. if you use openrc, ensure to launch hyprland with dbus-run-session Hyprland. Omitting the dbus-run-session may cause [`runtime errors`](https://wiki.gentoo.org/wiki/Sway#Failed_to_connect_to_user_bus)
5. `fonts` you need fontawesome and nerd-fonts use (3270 + symbols) (available in overlay) to display some icons in waybar

