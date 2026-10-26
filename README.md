# glibc sidecar

Release assets only: `glibc-aarch64.squashfs` and `glibc-armhf.squashfs` (with `.md5` and `.VERSION`), the glibc userland REG-Linux's musl boards mount on `/usr/glibc` and `/usr/glibc32` to run PortMaster ports.

`reglinux-portmaster install` downloads the release its image expects. To install by hand, put the three files of each arch in `/userdata/system/glibc/` and run `reglinux-portmaster install`.

Built from REG-Linux's `glibc-sidecar` recipe (`make glibc-sidecar-aarch64-build`, `make glibc-sidecar-armhf-build`); each release names the commit.
