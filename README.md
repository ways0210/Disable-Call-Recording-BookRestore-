# 📱 iOS Disable Call Recording (Unified Tool)

![iOS](https://img.shields.io/badge/iOS-18.0--26.1-blue)
![Status](https://img.shields.io/badge/Status-Stable-brightgreen)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS-lightgrey)
![Auto-Install](https://img.shields.io/badge/Auto--Install-Yes-success)
![Author](https://img.shields.io/badge/Author-YangJiii-orange)

A **unified, automated tool** to **replace or disable the call‑recording notification sound**
(**Start/Stop Disclosure**) on **iOS without Jailbreak**, using the **Books app file‑overwrite exploit**.

✨ **Now with Auto‑Dependency Installation & Enhanced UI!**

---

## 👤 Credits

- **Author:** YangJiii — [@duongduong0908](https://twitter.com/duongduong0908)  
- **Original Concept:** Huy Nguyen — @Little_34306

---

## ⚠️ DISCLAIMER & LEGAL NOTICE

### 1️⃣ Device & Data Risk
- This tool modifies **internal iOS system files**:
  ```
  /var/mobile/Library/CallServices/...
  ```
- Using system vulnerabilities **always carries risk**:
  - Boot loop
  - Soft brick
  - Data loss
- **The author takes NO responsibility** for any damage or data loss.
- **Use at your own risk.**

### 2️⃣ Legal Notice About Call Recording
- The *StartDisclosure* sound exists to comply with **privacy laws** in many countries.
- Disabling it **may violate local laws**.
- This project is for **educational & research purposes only**.
- **The author is not responsible for misuse.**

---

## 📂 Required Folder Structure

This tool is a **single‑file solution**. Your folder **MUST** look like this:

```
Your_Tool_Folder/
│
├── main.py          # Main script (Windows & macOS)
├── uuid.txt         # Auto‑generated (do NOT delete)
│
└── Sounds/
    ├── StartDisclosureWithTone.m4a
    └── StopDisclosure.caf
```

---

## 💻 Pre‑Requisites

### 1️⃣ Install Python 3
- Download from: https://www.python.org  
- ✅ **Check “Add Python to PATH” during installation**

### 2️⃣ Install iTunes (Windows Only)
- Required for Apple USB drivers  
- ⚠️ Avoid the Microsoft Store version if possible

### 3️⃣ Connect Your Device
- Connect iPhone via **USB**
- Tap **Trust This Computer** on the device

---

## 🚀 How To Run

✅ **No manual dependency installation needed!**  
The script automatically installs:
- `pymobiledevice3`
- `colorama`

---

### ▶️ Windows

1. Open the tool folder  
2. Type `cmd` in the address bar → **Enter**  
3. Run:

```bash
python main.py
```

🔑 *Recommended:* Run Command Prompt as **Administrator**

---

### ▶️ macOS / Linux

```bash
cd path/to/Your_Tool_Folder
python3 main.py
```

🔐 If prompted, enter your **macOS login password** to allow tunnel creation.

---

## 🛠️ How It Works

1. **Auto‑Install Dependencies**  
   Detects missing libraries, installs them, and restarts automatically.

2. **Device Detection**  
   Finds connected iPhone/iPad via USB.

3. **UUID Extraction**  
   Scans **Books app logs** to extract the hidden system UUID.

4. **Tunnel Creation (iOS 17+)**  
   Secure communication channel to the device.

5. **File Replacement**  
   Pushes **silent audio files** to iOS using backup/restore exploit logic.

---

## ❓ Common Issues & Fixes

### ❌ No device found
- Check USB cable
- Ensure iTunes (Windows) or Finder (macOS) detects device
- Tap **Trust** on iPhone

---

### ⏳ Stuck at “Searching for UUID…”
- Unlock iPhone
- Open **Books (Sách)** app
- Open any book (download a free sample if needed)

---

### 🔌 Tunnel creation failed
- Replug USB cable
- Reboot iPhone
- On macOS, ensure correct **sudo password**

---

### 🧱 Windows Installation Error
- Install **Microsoft Visual C++ Build Tools**
- Retry running the script

---

## ☕ Support

If this project helped you, consider supporting ❤️  

👉 **Ko‑fi:**  
https://ko-fi.com/yangjiii/goal?g=1

---

### ⭐ Star the project if you find it useful!
