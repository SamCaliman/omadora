# Frequently Asked Questions

## Where is the documentation for Omadora?

In general, Omadora reimplements much of the same functionality, keybindings, etc., that is in Omarchy, and therefore the [The Omarchy Manual](https://learn.omacom.io/) can be used as a guide for Omadora.

The [Hyprland Wiki](https://wiki.hypr.land) is also great reference documentation for the configuration of Hyprland.

However, the best resource for understanding Omadora is to read and understand the scripts within this repository with which you are executing.

## How do I keep Omadora updated?

There is an update indicator which appears in Waybar next to the date when an update is available; clicking this will pop a terminal and execute `omadora-update`.
The `omadora-update` script can also be run manually, and in both cases will update Omadora to the latest version, along with system packages, firmware, flatpaks, and cargo-installed binaries.

## Where are all the apps that are provided by default in Omarchy?

This is a conscious decision not to include all the applications and configuration options provided by Omarchy to minimise bloat and only install functionality that would be expected of a minimal desktop environment, leaving software installation choices to the user.

Many of these additional apps can be installed via the default official Fedora repositories or as a flatpak via [Flathub](https://flathub.org) if needed.

## Why are the Waybar glyphs so small with the default font?

The default font is the _Cascadia Mono NF_ font which is the only Nerd Font included within the offical Fedora repositories.
The glyphs in this font are the same width as the rest of the font which makes them appear small in comparison to other [Nerd Fonts](https://www.nerdfonts.com/font-downloads).

If larger glyphs are desired, then install the [CaskaydiaMono Nerd Font](https://www.nerdfonts.com/font-downloads#:~:text=CaskaydiaMono) or similar Nerd Fonts to the `~/.local/share/fonts` directory and rebuild the cache with `fc-cache -f`.
The fonts should now be available for selection via the Omadora style menu.

## Why have the default Omarchy themes been modified?

Neovim theme config files have been modified to load without the LazyVim plugin so that any Neovim configuration that uses the Lazy plugin manager can use the themes simply by symlinking in the theme plugin from `~/.config/omadora/current/theme/neovim.lua`.
However, third-party themes may still load the LazyVim plugin and would need to be modified manually after the theme install to work in the same manner.

## Where is the Omadora default plymouth theme from?

The default theme installed is from the great plymouth theme collection at [adi1090x/plymouth-themes](https://github.com/adi1090x/plymouth-themes).
