# 🔐 Nexus Offline Licensing System

A modular and secure offline licensing framework designed for Windows desktop applications.  
This system provides trial management, hardware-locked activation, and a standalone license generator for premium distribution.

> Built for personal software protection and controlled deployment.

<img src="https://github.com/markdweb/licensegenerator-v2/blob/master/src/cap.PNG" width="100%"/>

---

## 🏗️ System Architecture

The licensing ecosystem is composed of three core components:

1. **LicensingCore.dll** – Validation engine
2. **License Generator** – Admin tool for issuing licenses
3. **Client Application** – Protected Windows Forms app

All components work fully offline.

---

# 🧠 LicensingCore.dll

Core validation and licensing engine integrated into the protected application.

### Features

- 🔑 Hardware ID–locked licensing
- ⏳ Trial period management
- 🗓 Trial expiration tracking
- 📦 First-run detection via registry
- 🔐 Encrypted license file validation
- 🚫 Expired / invalid license blocking
- 👤 Client-bound license information
- 🎯 Premium vs Trial mode detection
- 🛡 Offline validation (no internet required)

### Security Design

- License tied to hardware fingerprint
- Encrypted license structure
- No plaintext license storage
- Registry-based trial enforcement

---

# 🛠 License Generator (Admin Tool)

Standalone desktop tool used to generate and manage licenses.

### Features

- 🧾 Client registration database (SQLite)
- 🔢 Hardware ID-based license creation
- 📅 Duration-based license generation
- 🏷 License status tracking
- 🔄 Renewal generation support
- 📂 Exportable license file creation
- 🧠 Premium license encoder
- 💾 Local database storage
- 🎨 Modern WinForms UI (Guna UI2)

Designed strictly for internal/private use.

---

# 💻 Client Application (Protected App)

The distributed Windows Forms application protected by LicensingCore.dll.

### Features

- 🟢 Premium mode detection
- 🔴 Trial mode with visible expiration date
- ⏰ Automatic trial expiration enforcement
- 🚪 Blocked access when expired
- 🔐 License activation system
- 📋 Hardware ID display for activation
- 🔄 Renewal flow support
- 💬 License status display (Licensed / Trial / Expired)
- 🎯 Automatic startup license validation

---

# 🔄 Licensing Flow

1. User installs application.
2. Trial begins automatically on first run.
3. Upon expiration, access is restricted.
4. User submits hardware ID.
5. Admin generates premium license.
6. User activates and unlocks premium mode.

All operations function completely offline.

---

# 🎯 Purpose

This project was created as a personal licensing framework to protect and control distribution of standalone Windows desktop applications.

It demonstrates:

- Secure offline licensing logic
- Hardware-locked activation
- Trial enforcement design
- Modular licensing architecture
- Professional desktop protection structure

---

# ⚙ Technologies Used

- C# (.NET Framework 4.8)
- Windows Forms
- SQLite
- Newtonsoft.Json
- Custom Encryption Logic

---

# 📌 Note

This system is designed for personal software distribution and educational purposes.

---

## 👤 Author

Mark Dhel Villarama  
Software Developer
