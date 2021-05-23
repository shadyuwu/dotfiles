# dotfiles

#install dmenu vim ranger

sudo pacman -S dmenu vim ranger

# install yay

cd ~
mkdir -p /tmp/yay_install
cd /tmp/yay_install

sudo pacman -S base-devel

sudo pacman -S expac yajl git

git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si

cd ~
rm -r /tmp/yay_install


# install pywal

sudo pacman -S feh imagemagick python-pip python-pywal

# install polybar

sudo pacman -S cairo libxcb python2 xcb-proto xcb-util-image xcb-util-wm xcb-util-xrm jsoncpp
yay -S polybar-git

# font
yay -S otf-overpass

# ranger
sudo pacman -S w3m
ranger --copy-config=scope


