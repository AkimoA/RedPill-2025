# RedPill-2025

A 3D OpenGL "Matrix" screensaver for macOS 




[![RedPill-2025 Demo Video](https://img.youtube.com/vi/dM-aSSvJqhg/maxresdefault.jpg)](https://www.youtube.com/watch?v=dM-aSSvJqhg)


![Matrix Digital Rain](https://img.shields.io/badge/Matrix-Digital%20Rain-green?style=for-the-badge)
![macOS](https://img.shields.io/badge/macOS-13.0%2B-blue?style=for-the-badge)
![Architecture](https://img.shields.io/badge/Architecture-arm64%20%7C%20x86__64-orange?style=for-the-badge)



- **Universal binary** supporting both Apple Silicon and Intel Macs
- **Modern compatibility** fixes for macOS Sonoma, Sequoia, and future versions
- **macOS 13.0** (Ventura) or later
- **Architecture:** arm64 (Apple Silicon) or x86_64 (Intel)

##  Installation

### Option 1: Direct Installation
1. Download the latest `RedPill.saver` from [Releases](../../releases)
2. Double-click the `.saver` file to install
3. Open **System Settings** → **Desktop & Screen Saver**
4. Select **Red Pill** from the screensaver list

### Option 2: Manual Installation
1. Copy `RedPill.saver` to one of these locations:
   ```bash
   ~/Library/Screen Savers/          # User installation
   /Library/Screen Savers/           # System-wide installation
   ```
2. Open **System Settings** → **Desktop & Screen Saver**
3. Select **Red Pill** from the screensaver list

## macOS Security Notice

### "Screensaver can't be opened" Error

If you see this message: *"Screensaver can't be opened because Apple cannot check it for malicious software"*

**Solution:**
1. Open **System Settings** → **Privacy & Security**
2. Scroll down to **Security** section
3. Click **"Allow Anyway"** next to the RedPill.saver notification
4. Return to **Desktop & Screen Saver** settings
5. Select **Red Pill** again
6. Click **"Open Anyway"** when prompted

This is normal for unsigned screensavers and is safe to allow.

## Building from Source

### Prerequisites
- **Xcode 15.0** or later
- **macOS 15.6.1** development environment
- **Command Line Tools** installed

### Build Steps
```bash
# Clone the repository
git clone https://github.com/yourusername/RedPill-2025.git
cd RedPill-2025

# Open in Xcode
open RedPill.xcodeproj

# Build (⌘+B) or use command line:
xcodebuild -project RedPill.xcodeproj -target RedPill -configuration Release build
```

### Installation After Building
```bash
# Copy built screensaver to your library
cp -R ~/Library/Developer/Xcode/DerivedData/RedPill-*/Build/Products/Release/RedPill.saver ~/Library/Screen\ Savers/
```

##  Troubleshooting

### legacyScreenSaver Process Issues
This version includes **automatic fixes** for the infamous `legacyScreenSaver` process that would consume CPU/memory after screensaver exit. The fixes are version-specific:

- **macOS Sonoma/Sequoia:** Uses proven `exit(0)` termination
- **macOS 26+ (Tahoe):** Uses delayed termination workaround


### Black Screen Issues
If the screensaver shows only a black screen:
1. Check **Privacy & Security** settings (see Security Notice above)
2. Ensure your Mac supports **Metal graphics**
3. Try restarting the **System Settings** app
4. Check **Console.app** for error messages

### Performance Issues
- The screensaver targets **60 FPS** but will adapt to your hardware
- On older machines, frame rate may be automatically reduced
- Memory usage should remain stable during long sessions



## License & Credits

### Copyright
- **© 2002-2012** mathew ([meta@pobox.com](mailto:meta@pobox.com)) - Original creator
- **© 2016** px3 ([rr@rdsroot.net](mailto:rr@rdsroot.net)) - First modernization 
- **© 2020** Jason Short - macOS 10.15 compatibility
- **© 2025** AkimoA - macOS 26.x.x compatibility & Legacy Screensaver Workaround from Aerial Project ( Thank you ) 

### License
This project is free software licensed under the **GNU General Public License v3.0**.

You can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but **WITHOUT ANY WARRANTY**; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the [GNU General Public License](LICENSE) for more details.


##  Links
- **Previous Fork:** [Jason Short's RedPill2](https://github.com/jasonshortphd/RedPill2)
- **GNU GPL License:** [https://www.fsf.org/](https://www.fsf.org/)
- **Report Issues:** [GitHub Issues](../../issues)

---

