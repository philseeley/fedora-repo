# Documentation

[Boat Instrument](https://philseeley.github.io/docs/boatinstrument/main.html)

# Repository Setup

Subscribe to the Fedora repository:

```shell
sudo echo if password required

cat <<__EOF | sudo tee /etc/yum.repos.d/phil-seeley.repo >/dev/null
[phil-seeley]
name=Phil Seeley Fedora \$releasever - \$basearch
baseurl=https://philseeley.github.io/fedora-repo/\$releasever/\$basearch/
enabled=1
gpgcheck=1
gpgkey=https://philseeley.github.io/fedora-repo/phil.seeley.gpg.pem
__EOF
```

# Desktop Installation

Fedora 41 and 42 are supported for x86_64.

```shell
sudo dnf install boatinstrument
```

If using a menu driven desktop (e.g. LXDE), the Boat Instrument can be found in the Utilities menu.

