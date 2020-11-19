# Welcome to EFI-hackintash decorative
Here are some hackintosh branch startups


##  Downloading macOS Big Sur

from isoriver [click download](https://isoriver.com/download-your-file-now/?url=https://archive.org/download/macOS.11.BigSur/macOS.11.BigSur.dmg)

## Create macOS **Big Sur** usb bootable
```
sudo /Applications/Install\ macOS\ Big\ Sur.app/Contents/Resources/createinstallmedia \
--volume /Volumes/MyVolume
```


## Create EFI and Mounted

```
git clone https://github.com/corpnewt/MountEFI
cd MountEFI
chmod +x MountEFI.command
```

## Copy EFI 

```
git clone https://github.com/abrahamfast/EFI-hackintash.git
cp EFI-hackintash/efi /Volumes/efi/
```

## Setup BIOS

 - Disable CSM
 - Disable Secure Boot
 - Set OS Type to Other OS
 - Set SATA as AHCI
 - Disable CFG Lock
 - Disable Intel Virtualization Technology / VT-X **
 - Disable VT-D **
 - Enable XHCI Hand-off
 - Disable Legacy USB Support **
 - Disable USB Keyboard and Mouse Simulator **


## Troubleshooting
See [OPENCORE](https://dortania.github.io/troubleshooting/)
