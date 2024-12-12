[![](https://img.shields.io/badge/EFI-Release-informational?style=flat&logo=apple&logoColor=white&color=9debeb)](https://github.com/Lorys89/ASROCK_Z490M-ITX-AC/releases)

# ASROCK Z490M ITX/AC Hackintosh Sequoia

EFI for ASROCK Z490M ITX/AC with OpenCore bootloader

### Computer Spec:

| Component        | Brank                                                  |
| ---------------- | ------------------------------------------------------ |
| CPU              | Intel Core ES QBT1 i9-10900 (10C-20T 20MB CML)         |
| iGPU             | Intel® UHD Graphics 630                                |
| GPU              | SAPPHIRE NITRO+ 580 8 GB                               |
| Lan 2.5 GBPS     | Realtek 8125                                           |
| Lan 1.0 GBPS     | Intel I219 V11                                         |
| Audio            | Realtek ALC1200                                        |
| Ram              | KINGSTON FURY BEAST 64GB (2 x 32GB) DDR4 3200 MHz CL16 |
| Wifi + Bluetooth | Intel 3168NGW                                          |
| 1° NVMe SSD      | CRUCIAL P3 PLUS 1 GB (MACOS/WIN11)                     |
| SmBios           | iMac 20,1                                              |
| BootLoader       | OpenCore 1.0.3                                         |
| macOS            | Sequoia 15.1.1                                         |


![infomac](./Screenshot/GPU-INFOMAC.png)
![infomac2](./Screenshot/IGPU-INFOMAC.png)


## Peripherals & Bench

![DEVICE](./Screenshot/PERIPH.png)
![PCI-LIST](./Screenshot/PCI-LIST.png)
![WIFI-TEST](./Screenshot/WIFI-SPEED.png)
![Fan&Temp](./Screenshot/SENSOR.png)


## USB Port Map

![Usb-Map](./Screenshot/USB-MAP.png)
![Usb-Map1](./Screenshot/USB-IO.png)
![Usb-Map2](./Screenshot/USB-INT.png)



### What works and What doesn't or WIP:

- [x] Intel UHD iGPU HDMI/DP Output
- [x] Intel UHD iGPU - H264 & HEVC
- [x] SAPPHIRE NITRO+ 580 HDMI/DP OUTPUT (with audio) 
- [x] SAPPHIRE NITRO+ 580 - H264 & HEVC
- [x] ALC1200 jack headphone (Front) 
- [x] ALC1200 jack line-out (Rear) 
- [x] ALC1200 jack microphone (Front & Rear)
- [x] ALC1200 jack linee-in (Rear) 
- [x] ALC1200 HDMI/DP Audio Output (IGPU)
- [x] All USB Ports (port mapping performed)
- [x] SpeedStep / Sleep / Wake
- [x] HID Key PWRB & SLPB 
- [x] Wi-Fi and Bluetooth Intel 3168NGW (Wi-Fi via HeliPort)
- [x] 1° CONTROLLER NVME PciE Gen3x4
- [x] 2° CONTROLLER NVME PciE Gen3x4
- [x] CONTROLLER SATA AHCI
- [x] All Sensors (CPU, GPU, NVME, SATA, FANS)
- [x] Realtek RTL8125 LAN
- [x] Intel I219 V11 LAN
- [x] NVRAM
- [x] Windows 11 boot from OpenCore
- [ ] Apple Continuity because of lack of support in latest macOS without OCLP



See [ioreg](./iMac_20,1.ioreg) for more clarification

### MacOS bootable USB creation:
- Read the Dortania guide for creating your USB from Windows or macOS
- [Guide Dortania](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/) - USB creation

### Additional tools
 * HeliPort for Wi-Fi

## Bios settings
### Enable :
* SATA Operation : AHCI
* XHCI Hand-Off
* XMP 2.0 Profile 1 or AUTO
* Primary Graphics Adapter : AUTO
* Share Memory : 128Mb
* IGPU Multi-Monitor

### Disable : 
* Secure Boot
* Intel SGX
* Fastboot
* CFG LOCK
* Boot From Onboard LAN
* CSM

## Credits

- [Apple](https://apple.com) for macOS;
- [Acidanthera](https://github.com/acidanthera) for OpenCore and all the lovely hackintosh work.
- [Lorys89](https://github.com/Lorys89) for Ventura version of this package
