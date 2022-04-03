# Suckless Desktop Environment

## Installation

### Dependencies
There are a few dependencies to compile the dependencies. Most are basic ones,
like having a C compiler, but you also need the following

```bash
sudo apt install libx11-dev libxft-dev libxinerama-dev libwebkit2gtk-4.0-dev libgcr-3-dev
```

### Installing the suckless tools

```bash
cd dwm && make && sudo make install && cd ..
cd dmenu && make && sudo make install && cd ..
cd st && make && sudo make install && cd ..
```

### Configuring with a desktop manager
1. Copy the `dwm.desktop` to `/usr/share/xsessions`
2. Copy the `startdwm` to `/usr/local/bin/startdwm` and make it executable
3. Log out and start DWM through your desktop manager

### Configuring without a desktop manager
1. Copy the `xinitrc` to `$HOME/.xinitrc`
2. Start by running `startx $HOME/.xinitrc`

