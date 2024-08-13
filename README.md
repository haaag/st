## st - simple terminal

st is a simple terminal emulator for X which sucks less.

## Prerequisites

- void

```sh
xbps-install libXft-devel libX11-devel harfbuzz-devel libXext-devel libXrender-devel libXinerama-devel
```

- debian (and ubuntu probably)

```sh
apt install build-essential libxft-dev libharfbuzz-dev
```

- arch

```sh
pacman -S gd
```

Install font-symbola and libXft-bgra

## Fonts

- Install [Maple Mono Font](https://github.com/subframe7536/maple-font/releases)

## Installation

Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

```sh
sudo make install
```

## Running st

If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

```sh
tic -sx st.info
```

See the man page for additional details.

## Credits

Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

```

```
