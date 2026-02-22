# 🔐 Bash Android AIO Bypass Kit

<div align="center">

[![Platform](https://img.shields.io/badge/Platform-Android-brightgreen)]()
[![Version](https://img.shields.io/badge/Version-1.0-blue)]()

**Koleksi lengkap tools Android untuk bypass FRP, EDL, dan utilities lainnya**

</div>

---

## 📝 Deskripsi

**Bash Android AIO Bypass Kit** adalah koleksi komprehensif tools dan utilities untuk Android yang mencakup:
- **FRP Bypass** - Bypass Factory Reset Protection
- **EDL Tools** - Emergency Download mode utilities
- **Device Firmware** - File firmware untuk berbagai manufacturer
- **Flashing Tools** - Tools untuk flash ROM dan file lainnya

Toolkit ini mendukung berbagai device dari manufacturer ternama seperti Oppo, Vivo, Xiaomi, Meizu, MTK dan lainnya.

> ⚠️ **PERHATIAN**: Toolkit ini hanya untuk tujuan edukasi dan pemulihan device pribadi. Pengguna bertanggung jawab atas penggunaan tools ini.

---

## ✨ Fitur Utama

- ✅ **FRP Bypass Tools** - Tools untuk bypass Factory Reset Protection
- ✅ **EDL Mode Support** - Tools untuk emergency download mode
- ✅ **Multi-Device Support** - Support untuk 100+ model device Android
- ✅ **Comprehensive Firmware** - Koleksi firmware dari berbagai manufacturer
- ✅ **Flash Tools** - MTK Flashtool, Qualcomm tools, dan utilities lainnya
- ✅ **Easy Commands** - Script batch yang mudah digunakan
- ✅ **Documentation** - Panduan lengkap untuk setiap device

---

## 📱 Daftar Device yang Didukung

### Manufacturer Utama:

| Brand | Jumlah Device | Folder |
|-------|--------------|--------|
| **Oppo** | 40+ | `/Oppo/` |
| **Vivo** | 20+ | `/Vivo/` |
| **Xiaomi** | 50+ | `/Xiaomi/` |
| **Meizu** | - | `/Meizu/` |
| **MTK Devices** | - | `/MTK/` |
| **Qualcomm** | - | `/ADB Fastboot eMMCDL/Qcom/` |
| **LG** | - | `/LG/` |

### Contoh Device:
- Oppo: A31C, A31T, A33F, A37, A51F, A71 2018, F1, F1Plus_R9
- Vivo: x20, x20plus, X5Pro, Y35, Y53, Y55S, Y65, Y71
- Xiaomi: Mi 4c, Mi 4i, Mi 5, Mi Note, Redmi series

---

## 🛠️ Persyaratan

### Windows:
- Windows 7/8/10/11
- ADB (Android Debug Bridge)
- Fastboot
- MTK Flashtool (jika diperlukan)

### Linux/Mac:
- ADB
- Fastboot
- Bash shell

### Hardware:
- USB Cable (preferably original)
- PC/Laptop
- Device yang ingin di-flash/bypass

---

## 📥 Instalasi

### 1. Clone Repository
```bash
git clone https://github.com/widifirmaan/bash-android-aio-bypass-kit.git
cd bash-android-aio-bypass-kit
```

### 2. Persiapan Device
- Aktifkan **Developer Mode** (tap 7x pada Build Number di Settings)
- Aktifkan **USB Debugging**
- Hubungkan device ke PC via USB

### 3. Install ADB & Fastboot
**Windows:**
```bash
# Install via command atau download dari Android SDK Platform Tools
# https://developer.android.com/studio/releases/platform-tools
```

**Linux/Mac:**
```bash
# Ubuntu/Debian
sudo apt-get install adb fastboot

# macOS
brew install android-platform-tools
```

---

## 🚀 Cara Penggunaan

### Pengecekan Status Device
```bash
cd "ADB Fastboot eMMCDL"
./cekstatus
```

### Mode EDL
```bash
# Untuk Qualcomm devices
cd "ADB Fastboot eMMCDL/Qcom"
# Jalankan tools yang sesuai

# Untuk MTK devices
cd MTK/Flashtool
# Gunakan MTK Flashtool
```

### FRP Bypass
1. Buka folder device yang ingin di-bypass (misalnya `/Oppo/A31C/`)
2. Ikuti panduan di folder `/Guide/`
3. Jalankan command yang sesuai

### Flashing ROM
```bash
adb devices           # Cek device terdeteksi
adb reboot bootloader # Reboot ke bootloader
fastboot flash boot boot.img
fastboot flash system system.img
```

---

## 📁 Struktur Folder

```
bash-android-aio-bypass-kit/
│
├── README.md                          # File ini
├── ADB Fastboot eMMCDL/               # Tools untuk ADB, Fastboot, EDL
│   ├── cekstatus                      # Script pengecekan status device
│   ├── edl.cmd / edl - Copy.cmd       # EDL mode command
│   ├── android/                       # Android utilities
│   ├── Qcom/                          # Qualcomm-specific tools
│   ├── MTK/                           # MTK-specific tools
│   ├── SPD/                           # Spreadtrum tools
│   └── exynos/                        # Exynos tools
│
├── Guide/                             # Dokumentasi & panduan
│   └── EDL Command.txt                # Panduan EDL commands
│
├── LG/                                # LG device firmware & files
│   └── V30 Thin Q/
│
├── Meizu/                             # Meizu device files
│   ├── auth files                     # Authentication files
│   └── mz_init/
│
├── MTK/                               # MediaTek devices
│   ├── auth files                     # MTK authentication
│   ├── scatter files                  # MTK scatter files
│   └── Flashtool/                     # MTK Flashtool
│
├── Oppo/                              # Oppo devices (40+ models)
│   └── [Model folders]
│
├── Twrp/                              # TWRP recovery files
│
├── Vivo/                              # Vivo devices (20+ models)
│   └── [Model folders]
│
└── Xiaomi/                            # Xiaomi devices (50+ models)
    ├── [Model folders]
    └── Redmi series
```

---

## ⚙️ Tools yang Disertakan

| Tool | Fungsi | Platform |
|------|--------|----------|
| **ADB** | Android Debug Bridge - komunikasi device | Windows/Linux/Mac |
| **Fastboot** | Flash mode commands | Windows/Linux/Mac |
| **EDL Tool** | Emergency Download mode | Qualcomm |
| **MTK Flashtool** | Untuk flash MTK devices | Windows |
| **Batch Scripts** | Automation commands | Windows |

---

## 📖 Panduan Khusus per Device

### Oppo Devices
1. Masuk folder `/Oppo/[Model]/`
2. Ikuti panduan yang ada di folder
3. Gunakan EDL atau Fastboot sesuai instruksi

### Xiaomi Devices
1. Aktifkan MI Account dan Developer Mode
2. Gunakan MiFlash atau fastboot commands
3. Lihat folder `/Xiaomi/[Model]/`

### Vivo Devices
1. Bypass FRP menggunakan tools di `/Vivo/[Model]/`
2. Gunakan Vivo Flash Tool jika diperlukan

### MTK Devices
1. Gunakan MTK Flashtool dari `/MTK/Flashtool/`
2. Load scatter file (.txt) dari `/MTK/`
3. Select ROM files dan flash

---

## ⚠️ Peringatan & Disclaimer

- **⚠️ Backup data Anda sebelum melakukan proses**
- Tools ini HANYA untuk device pribadi Anda
- Penggunaan tidak sah adalah **ILEGAL**
- Penulis TIDAK bertanggung jawab atas:
  - Data loss
  - Device damage
  - Banned account
  - Penggunaan ilegal
- **Gunakan dengan risiko sendiri**

---

## 🔧 Troubleshooting

### Device tidak terdeteksi ADB
```bash
# Windows
adb kill-server
adb start-server
adb devices

# Linux/Mac
sudo adb kill-server
sudo adb devices
```

### Device stuck di bootloader
- Hubungkan kembali ke PC
- Gunakan EDL mode recovery
- Flash stock ROM

### Fastboot connection error
- Install USB driver yang sesuai
- Gunakan cable original
- Coba port USB yang berbeda

---

## 📚 Resource Tambahan

- [Android SDK Platform Tools](https://developer.android.com/studio/releases/platform-tools)
- [ADB Documentation](https://developer.android.com/tools/adb)
- [Fastboot Guide](https://android.googlesource.com/platform/system/core/+/master/fastboot/)
- [XDA Developers](https://xda-developers.com)

---

## 🤝 Kontribusi

Kontribusi dirangkul! Jika Anda ingin menambah:
- Device firmware baru
- Tools tambahan
- Dokumentasi lebih lengkap

Silakan buat Pull Request atau Issue.

---

## 👨‍💻 Author

**Bash Android AIO Bypass Kit** - Created untuk komunitas Android

---

<div align="center">

**⭐ Jika tools ini membantu Anda, berikan star!** ⭐

*Last Updated: February 2026*

</div>
