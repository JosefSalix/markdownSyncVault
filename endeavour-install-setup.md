#### Alias
Vytvor si alias na: `sudo pacman -S --needed`

#### Development

```bash
sudo pacman -S --needed \
base-devel \
git \
ghc \
cabal-install
```

#### Xmonad

```bash
sudo pacman -S xmonad xmonad-contrib xmonad-extras
sudo pacman -S dmenu polybar rofi lxappearance
sudo pacman -S picom nitrogen feh scrot
sudo pacman -S xorg-xprop xorg-xset xorg-xrandr
sudo pacman -S xorg-server xorg-xinit xorg-xsetroot
sudo pacman -S lm_sensors xclip
sudo pacman -S dunst network-manager-applet
sudo pacman -S volumeicon playerctl pavucontrol
sudo pacman -S brightnessctl unzip unrar
sudo pacman -S pipewire pipewire-pulse pipewire-alsa wireplumber
```

#### Fonts

```bash
sudo pacman -S ttf-nerd-fonts-symbols
sudo pacman -S ttf-jetbrains-mono-nerd
sudo pacman -S ttf-fira-code-nerd
sudo pacman -S ttf-hack-nerd
sudo pacman -S ttf-ubuntu-mono-nerd
sudo pacman -S ttf-ubuntu-mono-nerd
sudo pacman -S ttf-dejavu-nerd
sudo pacman -S ttf-liberation-mono-nerd
sudo pacman -S ttf-cascadia-code-nerd
sudo pacman -S ttf-sourcecodepro-nerd
sudo pacman -S ttf-inconsolata-nerd
sudo pacman -S ttf-iosevka-nerd
sudo pacman -S ttf-font-awesome ttf-dejavu noto-fonts
```

#### Apps

```bash
sudo pacman -S emacs kitty chromium
sudo pacman -S gnome-characters
```

#### Wifi

```bash
sudo pacman -S gnome-keyring seahorse
```

#### Desktop entry (maybe)

```bash
sudo emacs /usr/share/xsessions/xmonad.desktop

[Desktop Entry]
Name=XMonad
Comment=Lightweight tiling window manager
Exec=xmonad
Type=Application
```

