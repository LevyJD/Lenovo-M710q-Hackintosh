
# Lenovo-M710q-Hackintosh
EFI for Lenovo M710q (10MR) with OpenCore 1.0.4 bootloader  

### Computer Spec:

| Component        | Specifications                         |
| ---------------- | ---------------------------------------|
| Model            | 10MR0004US                             |
| CPU              | Intel® Core™ i5-7500T                  |
| iGPU             | Intel® UHD Graphics 630                |
| RAM              | 2 * 16GB DDR4 2400 Mhz                 |
| LAN              | Intel I219-V                           |
| Audio            | Realtek ALC294                         |
| WiFi & Bluetooth | Intel 8265/8275                        |
| SMBIOS           | MacMini8,1                             |
| MacOS            | Ventura 13.7.4                         |
| BootLoader       | OpenCore 1.4.0                         |


### Instructions
- Generate your own SN/UUID/MLB/ROM
- In BIOS, disable CSM, set VRAM to 64MB, Enable VD-d, Set SATA to AHCI

### What Works:

- [x] Intel Intel® UHD Graphics 630 iGPU DP Output
- [x] ALC294 Internal Speakers
- [x] ALC294 & DP Audio Output
- [x] ALC294 Audio Input
- [x] All USB Ports
- [x] Intel I219-V
- [x] Intel Wi-Fi & Bluetooth
- [x] NVRAM

###  What Doesn't Work:

I can't upgrade to Sonoma / Sequoia. The Installer loads up fine, and the installation progresses to the first restart. After that it gets stuck in a boot loop at:

```
#[EB.LD.OFS|OPEN!] Err(0xE) <"usr\\standalone\\OS.dmg.root_hash"> 
```