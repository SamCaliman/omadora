# Omadora

This is a minimal functional install of Hyprland for Fedora 43 Workstation, based on the Omarchy implementation and patterns.
It provides a more stable release cycle with tested and curated packages.

Omadora purposely does not include all the apps and features included with Omarchy, as it's intended to be a minimal install that provides core desktop functionality to allow users to build from.
However, as the implementation closely matches Omarchy, adding extra features from Omarchy should be simple if you wish to do so.

Read more about Omarchy itself at [omarchy.org](https://omarchy.org).

## WTF (Why the fork)??
This fork was make because i need NetworkManger for my vpn apps to work, and i wanted a simpler install with a default fedora image.

## Important

Omadora attempts to install only packages from the official Fedora repositories, currently with the exception of a few Hyprland related packages, and mise.
These are provided by the [solopasha/hyprland](https://copr.fedorainfracloud.org/coprs/solopasha/hyprland/) and [jdxcode/mise](https://copr.fedorainfracloud.org/coprs/jdxcode/mise/) COPRs respectively, and as such, users should perform their own due diligence to ensure these are safe to install.

#### important also
This fork adds the `--allowerasing` flag to the install command so that it works on the base fedora workstation instalation

## Installation

Install Fedora 43 workstation. and complete the setup
Similar to Omarchy, it is recommended to use drive encryption, disable root, and add a privileged user.

Install git (`sudo dnf install -y git`) and clone this repo to the `~/.local/share/omadora` directory.

```
git clone https://github.com/samCaliman/omadora ~/.local/share/omadora
```

Run `~/.local/share/omadora/install.sh` to install.

## Usage

Omadora does not use the seamless login implemented in Omarchy, therefore once logged in, start Omadora using `omadora`.

Stop Omadora by using the power menu or executing `omadora-cmd-stop` or `uwsm stop`.

## Frequently Asked Questions

Check out the [FAQ.md](FAQ.md).

## Contribution
#### support the original repo from elpritchos
buy him a coffe
https://github.com/elpritchos/omadora

## License

Omadora is released under the [MIT License](https://opensource.org/licenses/MIT).
