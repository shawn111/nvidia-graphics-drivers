nvidia driver source: ftp://download.nvidia.com/XFree86/

Debianize source:
 * https://launchpad.net/ubuntu/+source/nvidia-graphics-drivers-experimental-310
 * https://github.com/tseliot/nvidia-settings.git
 * https://launchpad.net/~xorg-edgers/+archive/ppa

Create deb package
===

1. $ dch -i # create new version item.
2. $ fakeroot debian/rules clean # regen-from-templates & download binary files from nvidia ftp site.
4. $ ... # debianize eg. bzr bd -S
