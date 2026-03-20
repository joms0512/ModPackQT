# ModPackQT Gateway

**ModPackQT Gateway** is the desktop companion app for [ModPackQT](https://modpackqt.com) — a professional web-based Modbus Master/Slave platform for industrial automation.

The Gateway app installs on your machine and bridges your **modpackqt.com** browser session to real Modbus devices on your local network. It supports both **Modbus TCP** and **Modbus RTU** (via WebSerial), with real-time register editing, simulation bots, live traffic logging, and AI-assisted device setup.

> 📦 All installer files are available on the [Releases](https://github.com/joms0512/ModPackQT/releases) page.

---

## ✨ Features

- 🖥️ **System Tray** — runs quietly in the background; accessible from the menu bar
- 🔄 **Auto-Update** — notifies you and installs updates automatically
- 📋 **Live Logs** — real-time gateway log output inside the app window
- 🔌 **Local Modbus Gateway** — connects your local Modbus devices to the ModPackQT cloud
- 🤖 **Bot Support** — Scheduler, Signal Profile, and Function Bots executed locally
- 🌐 **Supports All Platforms** — Windows, macOS, and Linux

---

## 🌐 Signing In to modpackqt.com

Before using the Gateway app, you need a ModPackQT account.

1. Open your browser and go to **[https://modpackqt.com](https://modpackqt.com)**
2. Click **Sign In** (top right) or **Get Started**
3. Create an account or sign in using your existing credentials (powered by Clerk)
4. Once signed in, you will land on the **Dashboard**
5. Navigate to the **Master** or **Slave** page to start working with Modbus devices

> ℹ️ Your account is linked to the Gateway app — the app connects to your session automatically using your User ID. No manual token entry is required.

---

## 🖧 Master & Slave Capabilities

### Modbus Master
- Connect to real Modbus TCP/IP devices on your local network
- Read and write all register types: **Coils**, **Discrete Inputs**, **Input Registers**, **Holding Registers**
- Create and save connection profiles for quick reconnection
- Real-time data graphing with configurable refresh rates
- AI Quick Setup — describe what you need in plain language and ModPackQT creates slaves, profiles, and test environments automatically

### Modbus Slave Simulator
- Create and manage multiple Modbus TCP slaves from your browser
- Set register values manually or drive them with simulation bots
- Supports multiple simultaneous slave instances on different ports

### Gateway Bridge
- The Gateway app runs a local Modbus TCP server on your machine
- It connects to your modpackqt.com session over a secure cloud relay
- Supports multiple gateways per account (named tunnel keys)
- Gateway self-updates its script automatically from the cloud — no manual reinstall needed for script updates

---

## 💻 Installation

### Windows

1. Go to the [Releases](https://github.com/joms0512/ModPackQT/releases) page
2. Download the latest `.exe` installer
3. Run the installer and follow the on-screen steps
4. If Windows SmartScreen shows a warning:
   - Click **More info**
   - Click **Run anyway**
5. ModPackQT Gateway will launch and appear in your system tray

---

### macOS

#### Step 1 — Install from DMG

1. Go to the [Releases](https://github.com/joms0512/ModPackQT/releases) page
2. Download the latest `.dmg` file
3. Open the `.dmg` file
4. Drag **ModPackQT Gateway** to the **Applications** folder

#### Step 2 — Handle Gatekeeper Warning

When you first open the app, macOS may show:

> **"ModPackQT Gateway" Not Opened** — "Apple could not verify 'ModPackQT Gateway' is free of malware..."

Click **Done** — do **not** click "Move to Trash".

> ℹ️ This warning appears because the app is not yet notarized with Apple. It is safe to use.

#### Step 3 — Allow the App to Open

**Option A — Right-click method:**
1. Open **Finder** → **Applications**
2. Right-click (or Control-click) **ModPackQT Gateway**
3. Select **Open**
4. Click **Open** when the Gatekeeper warning appears again

**Option B — System Settings method:**
1. Go to **System Settings → Privacy & Security**
2. Scroll down to find the blocked app message
3. Click **Open Anyway**

---

### Linux

#### AppImage (all distros)

1. Go to the [Releases](https://github.com/joms0512/ModPackQT/releases) page
2. Download the latest `.AppImage` file
3. Open a terminal and run:

```bash
chmod +x ModPackQT-Gateway-*.AppImage
./ModPackQT-Gateway-*.AppImage
```

#### Debian / Ubuntu (.deb)

```bash
sudo dpkg -i modpackqt-gateway_*.deb
```

---

## 🔗 Connecting the Gateway to Your Account

Once installed and running:

1. The Gateway app starts automatically and appears in your **system tray**
2. Open **[https://modpackqt.com](https://modpackqt.com)** and sign in
3. The Gateway connects to your account automatically — no token entry needed
4. On the **Master** or **Slave** page, your gateway status will show as **Connected**
5. You can now send Modbus commands from your browser to real devices on your local network

---

## 🔄 Updates

The Gateway app checks for updates automatically on startup.

- When a new version is available, you will see an **update notification** inside the app
- Click **Update** to download and install the latest version
- The app will restart automatically after updating

To update manually:
1. Go to the [Releases](https://github.com/joms0512/ModPackQT/releases) page
2. Download the latest installer for your platform
3. Run the installer — it will replace the existing version

> The Gateway's internal bridge script updates itself automatically from the cloud without requiring a full app reinstall.

---

## 📋 System Requirements

| Platform | Minimum Version |
|----------|----------------|
| Windows  | Windows 10 (64-bit) |
| macOS    | macOS 10.15 Catalina |
| Linux    | Ubuntu 18.04 or equivalent |

> No additional software (e.g. Node.js) needs to be installed by the user. The app bundles everything it needs.

---

## 📦 Releases

Each release on the [Releases](https://github.com/joms0512/ModPackQT/releases) page includes:

| File | Platform |
|------|----------|
| `ModPackQT-Gateway-Setup-*.exe` | Windows |
| `ModPackQT-Gateway-*.dmg` | macOS |
| `ModPackQT-Gateway-*.AppImage` | Linux |

Release notes and changelogs are included with each release.

---

## 🐛 Issues & Feedback

- Report bugs or request features via the [Issues](https://github.com/joms0512/ModPackQT/issues) tab
- Use the **Feedback** button inside the app or visit [modpackqt.com/info](https://modpackqt.com/info) to contact support
