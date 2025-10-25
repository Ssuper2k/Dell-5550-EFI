# 💻 EFI for Dell Precision 5550 (macOS)

This repository contains a custom OpenCore EFI configuration for running macOS on the **Dell Precision 5550** with the following hardware:

## 🧰 System Specs

- **CPU**: Intel Core i7-10875H  
- **iGPU**: Intel UHD 630 (1536MiB)  
- **SSD**: Samsung 960 Pro 512GiB (M.2 NVMe)  
- **RAM**: 32GiB (2×16GiB @ 2933MHz)  
- **dGPU**: Nvidia Quadro T2000 *(disabled for macOS)*  
- **Display**: 3840×2400 Touch Screen  
- **macOS Version**: Sequoia 15.71  
- **OpenCore Version**: 1.05  

---

## ✅ What Works

- **Wi-Fi**: Intel AX200 *(spoofed, requires OCLP patching)*
- **Bluetooth 5.0**: *(same AX200 card)*
- **Trackpad**
- **Volume controls**
- **Brightness controls**
- **Touch Screen**
- **Thunderbolt 3** over USB-C
- **All USB ports**

---

## ⚠️ Important Notes

- **SMBIOS**: Please generate your own SMBIOS data using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) to avoid iCloud and serial number conflicts.
- **OCLP**: Required for proper AX200 Wi-Fi functionality. See [OpenCore Legacy Patcher](https://dortania.github.io/OpenCore-Legacy-Patcher/) for details.

---

## 📁 Folder Structure

This repo contains the full EFI folder, including:
- `ACPI/`
- `Drivers/`
- `Kexts/`
- `OC/config.plist`

Make sure to mount your EFI partition and replace its contents with this folder.

---

## 🛠️ Credits

Thanks to the Hackintosh community and tools like OpenCore, Dortania guides, and GenSMBIOS.

---

## 📌 Disclaimer

This EFI is provided as-is for educational and testing purposes. Use at your own risk. Always back up your data before making system-level changes.

