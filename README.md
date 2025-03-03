# Documentation

TODO - [Boat Instrument](docs/boatinstrument/main.md)

# Repository Setup

Subscribe to the Fedora repository:

```shell
sudo echo if password required

cat <<__EOF | sudo tee /etc/yum.repo.d/phil-seeley.repo
[phil-seeley]
name=Phil Seeley Fedora $releasever - $basearch
baseurl=https://philseeley.github.io/debian-ppa/fedora/$releasever/$basearch/
enabled=1
gpgcheck=1
gpgkey=https://philseeley.github.io/debian-ppa/phil.seeley.gpg.pem
__EOF
```

# Installation

There are two flavours of installation, one for Desktop environments and one for dedicated instruments. The latter uses flutter-pi to render directly to the console without the need for X11/Wayland.

## Boat Instrument - Desktop

If you are running a desktop environment.

Fedora 41 is supported for x86_64.

```shell
sudo dnf install boatinstrument
```

If using a menu driven desktop (e.g. LXDE), the Boat Instrument can be found in the Utilities menu.

## Boat Instrument - flutter-pi

Not currently supported on Fedora.

