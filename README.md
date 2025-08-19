# Asus-Notebook-R541U-Hackintosh-Big-Sur

Made With OpCore-Simplified

# Specification:

| Components.      | Model.                                 |
| ---------------- | -------------------------------------- |
| Notebook         | ASUS Notebook R541UJ                   |
| CPU              | Intel Core i3 6006U                    | 
| iGPU             | Intel® HD Graphics 520                 |
| Audio            | Realtek ALC256                         |
| LAN              | Realtek RTL8402                        |
| RAM              | 4 GB DDR4 2133 Mhz or more depends on your pc|
| SSD              | your model                             |
| SMBIOS           | MacBookPro13,1                         |
| Bootloader       | OpenCore 0.8.8                         |

![infodp1](./Screenshot/1.png)


## Read:
I Only tested this efi with Big Sur
Using Monterey, Ventura Is Not Recommended

## TO DO aka THINGS THAT SHIT ITSELF:
- [ ] Try and fix sleep Somehow (Its hackintosh ofc its an error)  
- [ ] Fixing Random Freezes While watching yt  
- [ ] Touchpad randomly shits itself and randomly starts working again  



## NOTES:
Im Incuding drivers for usb tethering  
also will add 2nd efi with drivers for AzureWave AW-CE123H  
Will be marked as release 1.0.1

## IMPORTANT!!

1.  Map your USB ports using USBToolBox.

After mapping, you will get a file named: USBMap.kext.

Copy USBMap.kext into your Kexts folder.

Open ProperTree and then:

- Open your config.plist
- Press Ctrl + R to OC Snapshot
- Select your OC folder
- Press Ctrl + S to save the changes

2. GenSMBIOS

You Need to generate serial rom uuid etc

Use [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate these things  
  1. Select your plist  
  2. Generate SMBIOS Number should be MacBookPro13,1
  3. Generate the Rom
  4. Generate The UUID
  5. Quit
Done! Now You can Boot Into The Installer


# BIOS Settings

Before the setting, load default settings
Also Ver 310 is required

## Enable:
- Intel Virtualizzation Technology
- DVMT Pre Allocated --> 64MB

## Disable:
- VT-d
- Fast Boot *works for me turned on*
- CSM Support
- Secure Boot Control

# Devices Screenshots
![sc1](./Screenshot/2.png)

# What works and what doesn't:
- [x] Intel® HD Graphics 520 iGPU
- [x] Realtek ALC256 Internal Output
- [x] Realtek ALC256 HDMI Audio Output
- [x] USB Ports
- [x] Realtek RTL810xE
- [x] NVRAM
- [x] Boot Windows By OpenCore
- [x] SD Card Reader (works)
- [x] Top Row Keys (Brightness,volume etc.)
- [ ] NVIDIA® GeForce® 920M
- [ ] WiFi + Bluetooth (you can replace the card with a compatible one recomended AzureWave AW-CE123H)


## Credits
**Found a solution to the TODO list?**  
Feel free to contact me at: [gkkoxx2.gk@gmail.com](mailto:gkkoxx2.gk@gmail.com)
- [Acidanthera](https://github.com/acidanthera) for OpenCore Bootloader
- [Apple](https://apple.com) for macOS
- [Dortania](https://github.com/dortania) for OpenCore Guides
- [OpCore-Simplify](https://github.com/lzhoang2801/OpCore-Simplify) Made Efi
- i stole readme from [SASA-Tech](https://github.com/SASA-Tech/Asus-VivoBook-R541U-Hackintosh/tree/main)
