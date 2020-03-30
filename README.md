# Arc Theme Red

[![Donate](https://img.shields.io/badge/Donate-PayPal-blue.svg)](http://paypal.me/mclmza)

A red variation of [Horst3180's Arc Theme](https://github.com/horst3180/arc-theme).

This version has a reduced color range, is mostly gray and red. I developed this version especially for all those who use linux on a Thinkpad.

Download the built theme [here](https://github.com/mclmza/arc-theme-Red/releases/download/1/Arc-Red-theme.zip)

Arc is a flat theme with transparent elements for GTK 3, GTK 2 and Gnome-Shell which supports GTK 3 and GTK 2 based desktop environments like Gnome, Unity, Budgie, Pantheon, XFCE, Mate, etc.

### Arc Red is available in three variants 

##### Arc-Red

![A screenshot of the Arc theme](http://i.imgur.com/Utgi19P.png)

##### Arc-Red-Darker

![A screenshot of the Arc-Darker theme](http://i.imgur.com/dQbcAc1.png)

##### Arc-Red-Dark

![A screenshot of the Arc-Dark theme](http://i.imgur.com/z4Dg8pb.png)


### Requirements

* Gnome/GTK 3.14, 3.16, 3.18 or 3.20
* The `gnome-themes-standard` package
* The murrine engine. This has different names depending on your distro.
  * `gtk-engine-murrine` (Arch Linux)
  * `gtk2-engines-murrine` (Debian, Ubuntu, elementary OS)
  * `gtk-murrine-engine` (Fedora)
  * `gtk2-engine-murrine` (openSUSE)
  * `gtk-engines-murrine` (Gentoo)

Main distributions that meet these requirements are

* Arch Linux and Arch Linux based distros
* Ubuntu 15.04, 15.10 and 16.04 (**Ubuntu 14.04 and 14.10 are not supported**)
* elementary OS Freya
* Debian 8, Testing or Unstable
* Gentoo
* Fedora 21 - 24
* openSUSE 13.2, Leap 42.1 and Tumbleweed

Derivatives of these distributions should work, as well.

If your distribution isn't listed, please check the requirements yourself.

### Installation

**Important:** Remove all older versions of the theme from your system before you proceed any further.

    sudo rm -rf /usr/share/themes/{Arc-Red,Arc-Red-Darker,Arc-Red-Dark}
    rm -rf ~/.local/share/themes/{Arc-Red,Arc-Red-Darker,Arc-Red-Dark}
    rm -rf ~/.themes/{Arc-Red,Arc-Red-Darker,Arc-Red-Dark}

#### Packages

Prebuilt packages for Ubuntu, Debian, Fedora and openSUSE are available at ...

#### Manual Installation

To build the theme you'll need 
* `autoconf`
* `automake`
* `pkg-config` or `pkgconfig` if you use Fedora
* `libgtk-3-dev` for Debian based distros or `gtk3-devel` for RPM based distros
* `git` if you want to clone the source directory

If your distributions doesn't ship separate development packages you just need GTK 3 instead of the `-dev` packages.

Install the theme with the following commands

**1. Get the source**

If you want to install the latest version from git, clone the repository with

    git clone https://github.com/mclmza/arc-theme-Red --depth 1 && cd arc-theme-Red

**2. Build and install the theme**

    ./autogen.sh --prefix=/usr
    sudo make install

Other options to pass to autogen.sh are

    --disable-transparency     disable transparency in the GTK3 theme
    --disable-light            disable Arc Light support
    --disable-darker           disable Arc Darker support
    --disable-dark             disable Arc Dark support
    --disable-cinnamon         disable Cinnamon support
    --disable-gnome-shell      disable GNOME Shell support
    --disable-gtk2             disable GTK2 support
    --disable-gtk3             disable GTK3 support
    --disable-metacity         disable Metacity support
    --disable-unity            disable Unity support
    --disable-xfwm             disable XFWM support

    --with-gnome=<version>     build the theme for a specific Gnome version (3.14, 3.16, 3.18, 3.20)
                               Note: Normally the correct version is detected automatically and this
                               option should not be needed.
                               Note 2: For GNOME 3.24, use --with-gnome-version=3.22
                               (this works for now, the build system will be improved in the future)

After the installation is complete you can activate the theme with `gnome-tweak-tool` or a similar program by selecting `Arc-Red`, `Arc-Red-Darker` or `Arc-Red-Dark` as Window/GTK+ theme and `Arc-Red` or `Arc-Red-Dark` as Gnome-Shell and Xfce-Notify theme.

**Uninstall the theme**

Run

    sudo make uninstall

from the same directory as this README resides in, or

    sudo rm -rf /usr/share/themes/{Arc-Red,Arc-Red-Darker,Arc-Red-Dark}

### Todo

- Replace the color of some remaining pictures in the assets folder.

### Extras

#### Arc Red Docky theme
A theme for Docky is available at https://github.com/alireza-amirsamimi/Arc-Dark-Docky-themes

#### Arc icon theme
The Arc icon theme is available at https://github.com/horst3180/arc-icon-theme

### Troubleshooting

If you have Ubuntu with a newer GTK/Gnome version than the one included by default (i.e Ubuntu 14.04 with GTK 3.14 or Ubuntu 15.04 with GTK 3.16, etc.) the prebuilt packages won't work properly and you have to install the theme manually as described above.
This is also true for other distros with a different GTK/Gnome version than the one included by default

--

If you get artifacts like black or invisible backgrounds under Unity, disable overlay scrollbars with

    gsettings set com.canonical.desktop.interface scrollbar-mode normal


### Bug reporting
If you find a bug, please report it at https://github.com/mclmza/arc-theme-Red/issues

### Full Preview
![A full screenshot of the Arc Red theme](http://i.imgur.com/6dh5qvb.jpg)
<sub>Screenshot Details: Icons: Coming soon | [Wallpaper](https://www.walldevil.com/510903-red-galaxy-wallpaper.html) | Font: Cantarell</sub>
