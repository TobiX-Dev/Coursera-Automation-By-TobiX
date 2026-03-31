# Coursera Auto-Complete Extension

![Version](https://img.shields.io/badge/version-2.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Chrome](https://img.shields.io/badge/chrome-extension-4c8bf5)

**Automatically complete Coursera courses** with one click. Skip videos, readings, discussions, plugins, and even solve quizzes using AI. Get shareable links for peer‑graded assignments. Premium security with device binding, daily limits, and hard expiration.

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🎬 **Skip Videos** | Mark all video lectures as completed instantly. |
| 📖 **Skip Readings** | Complete all reading materials in one go. |
| 💬 **Skip Discussions** | Post a dummy reply to mark discussions as done. |
| 🔌 **Skip Plugins** | Automatically complete ungraded plugins (e.g., surveys). |
| 🤖 **Quiz Solver** | AI‑powered answers for single‑choice, multiple‑select, and text‑input questions (requires Groq API key). |
| 🔗 **Shareable Link** | Generate a review link for peer‑graded assignments (copy to clipboard). |
| 🔒 **Premium Security** | Device fingerprinting, daily verification limit, and hardcoded expiration to prevent abuse. |
| 🔓 **Free Tier** | Basic skip features available for everyone. |

## 🚀 Installation

1. **Download the latest release** from [GitHub Releases](https://github.com/TobiX-Dev/coursera-auto-complete/releases) or clone this repository.
2. **Unzip** the folder.
3. **Open Chrome** and go to `chrome://extensions/`.
4. **Enable Developer mode** (toggle in the top right).
5. **Click “Load unpacked”** and select the extension folder.
6. The extension icon will appear in the toolbar. Click it to open the popup.

## 🧑‍💻 Usage

### Free Features
- Click **“Skip Videos”**, **“Skip Readings”**, **“Skip Discussions”**, or **“Skip Plugins”** on any Coursera course page.
- Wait a few seconds – the items will be marked as completed. Refresh the page to see the checkmarks.

### Quiz Solver (Premium)
1. **Get a Groq API key** from [console.groq.com/keys](https://console.groq.com/keys) (free tier available).
2. **Enter the key** in the extension popup (Settings section) and save.
3. **Open a quiz** on Coursera.
4. **Click “Solve This Quiz”** in the popup.
5. The extension will fill the answers automatically. Confirm submission when prompted.

### Shareable Link (Premium)
1. **Go to the submission page** of a peer‑graded assignment (URL contains `/submit`).
2. **Click “Shareable Link”** in the extension popup.
3. The link is copied to your clipboard. Share it with your reviewer.

### Activate Premium License
1. **Obtain a license key** (contact the developer or purchase from the link inside the popup).
2. **Click “Unlock Extension”** and enter the key.
3. The extension will verify the key and activate premium features.

## 🔒 Security & Privacy

- **Device fingerprinting** (canvas + WebGL + random salt) ensures each key works only on one device.
- **Daily verification limit** (10 checks per day) prevents abuse.
- **Hardcoded expiration** (e.g., 6 months after release) forces users to update, breaking old copies.
- **No data collected** – all processing happens locally or via the Groq API (quizzes) and your license server.

## 🛠️ Development

### Build from source
1. Clone the repository.
2. Load the unpacked extension in Chrome (as above).
3. Modify `popup.js`, `content.js`, etc. and reload the extension to test.

### Obfuscation
For release, obfuscate the JavaScript files using [JavaScript Obfuscator](https://obfuscator.io/) with high settings (enable self‑defending, debug protection, control flow flattening). Minify `popup.html` using [HTMLMinifier](https://kangax.github.io/html-minifier/).

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

This tool is for **educational purposes only**. The developer is not responsible for any misuse or violation of Coursera’s terms of service. Use at your own risk.

## 🙏 Support

- **Buy a license** to support development and get premium features.
- **Report issues** on GitHub.
- **Star the repo** if you find it useful!

---
**Made with ❤️ by TobiX**
