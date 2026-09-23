# 🌐 Ultimate Web & PHP to EXE Compiler

A lightweight, powerful graphical interface that compiles local web projects (HTML, CSS, JS) and PHP applications into native, standalone Windows executables (`.exe`). 

Instead of forcing users to install local web servers or Python environments, this tool bundles everything they need into one runnable file, complete with custom window controls and SmartScreen metadata.

## ✨ Features

* **Full PHP Support:** Optionally bundle a portable PHP engine to run backend PHP scripts completely offline.
* **Smart Window Controls:** Toggle fullscreen, frameless windows, always-on-top, private mode, and more directly from the UI.
* **Auto-Dependency Setup:** The script automatically detects and installs required Python packages (`pywebview`, `PyInstaller`) on first run.
* **Anti-Cloning Protection:** Built-in safeguards (`multiprocessing.freeze_support()`) prevent the notorious PyInstaller "fork-bomb" crash.
* **SmartScreen Mitigation:** Automatically generates Windows version metadata to reduce false-positive security flags from Windows Defender.
* **Clean & Modern UI:** A responsive Tkinter dashboard built for ease of use.

## 🚀 Getting Started

### Prerequisites
To use this compiler, you need to have Python installed on your Windows machine.
1. Download Python from [python.org](https://www.python.org/)
2. **Important:** When installing Python, ensure you check the box that says **"Add Python to PATH"**.

### Installation
1. Clone this repository or download the source code as a ZIP file.
2. Run the `compiler.py` script. 
3. The app will automatically install its own dependencies (`PyInstaller` and `pywebview`) the first time it launches.

## 🛠️ How to Compile an App

1. **Select Web Folder:** Point the compiler to your project folder containing your `index.html` or `index.php` file, along with your CSS/JS assets.
2. **Select PHP Engine (Optional):** If you are compiling a PHP application, download the [Windows PHP Binaries](https://windows.php.net/download/), extract the ZIP, and select that folder here. (Skip this if you are only using HTML/JS).
3. **Configure Output:** Name your `.exe` file and give your application window a title.
4. **Select Features:** Check the boxes for how you want the app to behave (e.g., Full Screen, Disable Cache, No Frame Window).
5. **Build:** Click **Build Standalone Executable**. The app will safely package your code and open the output folder when finished!

## ⚠️ Important Note on PyInstaller
Because this tool uses PyInstaller to bundle applications, some overly strict antivirus software might flag the resulting `.exe` files as suspicious. This is a known false positive with PyInstaller. The compiler actively mitigates this by generating official version metadata, but users can whitelist the output folder if needed.

## 💝 Support the Developer
If this tool saved you hours of packaging headaches, consider supporting its development!
* **UPI (India):** `ernamaanshaid@oksbi`
* **PayPal (Global):** [Donate via PayPal](https://www.paypal.com/paypalme/namaanshahid)

## 📄 License
This project is open-source. It utilizes `pywebview` (BSD 3-Clause) and `PyInstaller` (GPL with Bootloader Exception) to generate applications.