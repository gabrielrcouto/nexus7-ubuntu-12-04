# Ubuntu 12.04 for Nexus 7 (2012)

This is an ARM version of Ubuntu 12.04 (LTS) patched with the lastest NVIDIA Tegra Drivers.

To install, copy the MROM file to you tablet and use MultiROM (http://forum.xda-developers.com/showthread.php?t=2011403).

You'll need an OTG cable to plug a keyboard on your tablet and setup it.

## First step

```sh
Username: ubuntu
Password: ubuntu
```

### Configure your wifi (WPA)

```sh
$ wpa_passphrase the_name_of_your_wifi_network the_passphrase > wpa.conf
$ wpa_supplicant -B -Dwext -iwlan0 -cwpa.conf
```

### Install desktop environment

```sh
$ sudo su
Password: ubuntu
$ apt-get update
$ apt-get install ubuntu-desktop gnome-session-fallback
```

After finishing, reboot and you'll see the LightDM screen.

## Using

I recommend you to use the "GNOME Classic (No effects)" session, it's light and doesn't have the touch bug, reported on https://bugs.launchpad.net/ubuntu-nexus7/+bug/1068994

![How to choose the session](http://4.bp.blogspot.com/-1uvXhmQZ5Ic/TzW7sfOJB3I/AAAAAAAAHuk/1NSdl4NJVZM/s1600/gnome-classic-login-screen.png)

## Author

Gabriel Couto - [@gabrielrcouto](http://www.twitter.com/gabrielrcouto)
