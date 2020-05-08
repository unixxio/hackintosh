# Hackintosh

This repo contains working **OpenCore** and **Clover** configurations for specific hardware. All the configurations are kept as clean as possible.

**Last updates** (DD-MM-YYYY):

* 08-05-2020 - Added OpenCore 0.5.8 for macOS Catalina for Intel NUC D34010WYK

## OpenCore
**Requirements**

* Pre-configured bootable USB with OpenCore (guides are easy to find online)
* [Binary Resources](https://github.com/acidanthera/OcBinaryData) must be placed in `EFI/OC/Resources` on your installation media.
* [MountEFI](https://github.com/corpnewt/MountEFI) to install OpenCore bootloader without needing the installation media.

**Instructions**

Before installing macOS:

* The **config.plist** files on this repo contain **example** **serialnumbers** and **UUID's**. Generate your own with [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) otherwise iServices such as iMessage will **not** work.
* Make sure your installation media contains the **Binary Resources** mentioned in the Requirements.

After installing macOS:

* Mount the macOS EFI partition with **MountEFI** and copy the EFI folder from your installation media (containing Binary Resources) to the EFI partition.
* Rename `config.plist` to `install.config.plist`
* Rename `post_install.config.plist` to `config.plist`

## Clover

No instructions yet.