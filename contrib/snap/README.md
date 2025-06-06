# Voltaem Snap Packaging

Commands for building and uploading a Voltaem Core Snap to the Snap Store. Anyone on amd64 (x86_64), arm64 (aarch64), or i386 (i686) should be able to build it themselves with these instructions. This would pull the official Voltaem binaries from the releases page, verify them, and install them on a user's machine.

## Building Locally
```
sudo apt install snapd
sudo snap install --classic snapcraft
sudo snapcraft
```

### Installing Locally
```
snap install \*.snap --devmode
```

### To Upload to the Snap Store
```
snapcraft login
snapcraft register voltaem-core
snapcraft upload \*.snap
sudo snap install voltaem-core
```

### Usage
```
voltaem-unofficial.cli # for voltaem-cli
voltaem-unofficial.d # for voltaemd
voltaem-unofficial.qt # for voltaem-qt
voltaem-unofficial.test # for test_voltaem
voltaem-unofficial.tx # for voltaem-tx
```

### Uninstalling
```
sudo snap remove voltaem-unofficial
```