# davinci-resolve-studio for Arch Linux
Archlinux Package to install Blackmagic's Davinci Resolve Studio, based on https://aur.archlinux.org/packages/davinci-resolve/

This package adds the package name and sha256 from the studio version zip file, and also adds an udev rule for the dongle. Please let me know of any [issues here](https://github.com/codibit/davinci-resolve-studio/issues).
## INSTALLATION:

To install, simply download the Davinci Resolve Studio installer from [Blackmagic's website](https://www.blackmagicdesign.com/products/davinciresolve/) to your Downloads directory. The DaVinci_Resolve_Studio_14.2.1_Linux.zip file (for the 14.2.1 version) should be placed into /home/$youruser/Downloads or inside the package directory.

### Automatic installation:
You should be able to automatically install from the AUR repository with a tool like [yaourt](https://archlinux.fr/yaourt-en):

`yaourt davinci-resolve-studio`

### Manual installation:
* If you want to manually install, clone this repository from [GitHub](https://github.com/codibit/davinci-resolve-studio) _or_ [AUR](https://aur.archlinux.org/packages/davinci-resolve-studio/):

`git clone https://github.com/codibit/davinci-resolve-studio.git`

_or_

`git clone https://aur.archlinux.org/davinci-resolve-studio.git`

* run makepkg inside the directory (as your regular user):

`cd davinci-resolve-studio`

`makepkg`

* and finally install the created package with pacman (as root):

`pacman -U davinci-resolve-studio-14.2.1-0-x86_64.pkg.tar.xz`

## TODO: 
I don't use BlackMagic's panels, so I didn't bother to add the BMDPanel support drivers & daemon. If someone could test it, I might add it to the package.

## CREDITS:
All the package credits go to the [davinci-resolve](https://aur.archlinux.org/packages/davinci-resolve/) package mantainer and contribuitors in [https://aur.archlinux.org/packages/davinci-resolve/](https://aur.archlinux.org/packages/davinci-resolve/)
