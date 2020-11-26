# Project LightK1SS-Sway
The goal of this project it to provide K1SS packages so that [Sway](https://github.com/swaywm/sway) can be installed on K1SS Linux using the default package manager.

## Tasks
### Create core dependency list-
Only unique dependencies are listed in branches of the dependency tree.

Dependency name | Compile-time (c) or Runtime (r) | Source location | Dependency of
--------------- | ------------------------------- | --------------- | -------------
meson | c | kiss/repo/extra | sway
wayland | r | http | sway
wayland-protocols | c | http | sway
pcre | r | community/community | sway
json-c | r | community/community | sway
pango (wayland-only) | r | http | sway
cairo (wayland only) | r | http | sway
gdk-pixbuf | r | kiss/repo/extra | sway
wlroots | r | http | sway
flex | c | kiss/repo/core | sway
samurai (?) | c | kiss/repo/extra | sway
scdoc (?) | r | community/community | sway
swaybg (?) | r | http | sway
expat | r | kiss/repo/extra | wayland
libffi | r | kiss/repo/extra | wayland
libxml2 | r | community/community | wayland
NULL | NULL | NULL | wayland-protocols
edudev | r | kiss/repo/extra | wlroots
libdrm | r | kiss/repo/extra | wlroots
libxkbcommon | r | kiss/repo/xorg | wlroots
libinput | r | kiss/repo/extra | wlroots
linux-headers | c | kiss/repo/core | wlroots
mesa (wayland only) | r | http | wlroots
pixman | r | kiss/repo/xorg | wlroots
xkeyboard-config | r | kiss/repo/xorg | wlroots
bison | c | kiss/repo/core | mesa (wayland only)
expat | r | kiss/repo/extra | mesa (wayland only)
libdrm | r | kiss/repo/extra | mesa (wayland only)
libelf | r | kiss/repo/extra | mesa (wayland only)
libglvnd | r | http | mesa (wayland only)
linux-headers | c | kiss/repo/core | mesa (wayland only)
llvm __(!!)__ | r | kiss/repo/extra | mesa (wayland only)
m4 | c | kiss/repo/core | mesa (wayland only)
python | c | kiss/repo/extra | mesa (wayland only)
zlib | r | kiss/repo/core | mesa (wayland only)
libXext | r | kiss/repo/xorg | libglvnd
libX11 | c | kiss/repo/xorg | libglvnd
xorgproto | c | kiss/repo/xorg | libglvnd
python | c | kiss/repo/extra | libglvnd
NULL | NULL | NULL | swaybg