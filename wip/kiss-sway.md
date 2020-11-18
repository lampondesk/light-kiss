# Project K1SS-Sway
The goal of this project it to provide K1SS packages so that [Sway](https://github.com/swaywm/sway) can be installed on K1SS Linux using the default package manager. This is still WIP, and if successful, I might ask for K1SS Linux maintainer Dylan Araps for my packages to be added to the [community repo](https://github.com/kisslinux/community).

## Tasks
### Create dependency list
Dependency name | Compile-time (c) or Runtime (r) | Source location | Dependency of
--------------- | ------------------------------- | --------------- | -------------
meson | c | kiss/repo/extra | sway
wayland | r | git | sway
wayland-protocols | c | git | sway
pcre | r | svn | sway
json-c | r | ? | sway
pango | r | ? | sway
cairo | r | ? | sway
gdk-pixbuf2 | r | ? | sway
wlroots | r | git | sway
mesa w/ wayland platform | r | http | wlroots
libdrm | r | kiss/repo/extra | wlroots
xkbcommon | r | ? | wlroots
udev _(eudev?)_ | r | kiss/repo/core _(?)_ | wlroots
pixman | r | ? | wlroots