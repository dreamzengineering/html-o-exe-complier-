# Ultimate HTML/PHP-to-EXE Compiler

An open-source Python desktop application built with Tkinter that packages web projects (HTML, CSS, JavaScript, and PHP) into standalone Windows executables (`.exe`). It combines `pywebview` for rendering the native application window and `PyInstaller` for single-file compilation, with integrated support for bundling a portable PHP development server.

---

## 🌟 Key Features

* **Single-File Compilation:** Bundles web assets and dependencies into a self-contained `.exe` binary.
* **Embedded PHP Runtime Support:** Automatically launches a background PHP CLI web server (`php.exe -S 127.0.0.1:<port>`) on an available local port for processing `.php` scripts.
* **Window Feature Matrix:** Customizable UI flags including Fullscreen, Resizable, Maximize, Always-on-Top, Private Mode, and Frameless Window.
* **Auto-Dependency Bootstrap:** Detects missing packages (`pyinstaller`, `pywebview`) on startup and automatically installs them via `pip`.
* **SmartScreen Metadata Generator:** Automatically writes `version_info.txt` metadata (Company, Product Version, Copyright) to minimize Windows SmartScreen flags.
* **Thread-Safe Build Execution:** Utilizes background threading and safe UI updates to maintain responsiveness during the PyInstaller build process.

---

## 📋 Prerequisites

* **Operating System:** Windows 10 or Windows 11
* **Python Environment:** Python 3.8 or higher (ensure Python is added to your system `PATH`)
* **PHP Engine (Optional):** A portable Windows build of PHP (a directory containing `php.exe`), required only if compiling PHP projects.

---

## 🚀 Installation & Setup

1. **Clone or Download the Repository:**
   Save the main exe and run it

2. **Install Dependencies:**
   The application automatically detects and installs missing dependencies on launch. Alternatively, you can manually install them using `pip`:
   ```bash
   pip install pyinstaller pywebview

   💝 Support the Developer
If this tool saved you hours of packaging headaches, consider supporting its development!
UPI (India): `ernamaanshaid@oksbi`
PayPal (Global): Donate via PayPal
📄 License
This project is open-source. It utilizes `pywebview` (BSD 3-Clause) and `PyInstaller` (GPL with Bootloader Exception) to generate applications.
