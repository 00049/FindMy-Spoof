# 📍 LocationSnhika — Xcode GPS Spoofer

> Simulate any GPS location on iOS using Xcode's built-in location simulation feature. No jailbreak. No third-party tools. Just a `.gpx` file.

---

## 🗺️ What is this?

**LocationSnhika** is a `.gpx` file that lets you fake your iPhone or iPad's GPS location directly from Xcode — useful for testing location-based apps, games, or features without physically moving.

Currently set to 📌 **Greater Noida, India** (`28.4501° N, 77.5845° E`)

---

## 🖥️ Requirements

| Tool | Version |
|------|---------|
| macOS | 12.0+ |
| Xcode | 13.0+ |
| iOS Device / Simulator | Any |

---

## 🚀 How to Use

### Step 1 — Clone the repo

```bash
git clone https://github.com/yourusername/LocationSnhika.git
```

### Step 2 — Open Xcode and run your app

Open any Xcode project and build it on a **simulator or connected device**.

> 📸 *[Screenshot: Xcode with app running on simulator]*

---

### Step 3 — Add the GPX file to Xcode

Go to:
```
Debug → Simulate Location → Add GPX File to Project...
```

Select `newlocation.gpx` from the cloned folder.

> 📸 *[Screenshot: Debug menu → Simulate Location]*

---

### Step 4 — Activate the location

Once added, click:
```
Debug → Simulate Location → Greater Noida
```

Your device/simulator will now report its location as **Greater Noida, India**. ✅

> 📸 *[Screenshot: Maps app showing spoofed location]*

---

## 📄 The GPX File

```xml
<?xml version="1.0"?>
<gpx version="1.1" creator="Xcode">
    <wpt lat="28.4501" lon="77.5845">
        <name>Greater Noida</name>
    </wpt>
</gpx>
```

---

## ➕ Adding More Locations

You can easily add more waypoints to the GPX file:

```xml
<?xml version="1.0"?>
<gpx version="1.1" creator="Xcode">
    <wpt lat="28.4501" lon="77.5845">
        <name>Greater Noida</name>
    </wpt>
    <wpt lat="28.6139" lon="77.2090">
        <name>New Delhi</name>
    </wpt>
    <wpt lat="19.0760" lon="72.8777">
        <name>Mumbai</name>
    </wpt>
</gpx>
```

Each `<wpt>` entry will appear as a separate option under **Debug → Simulate Location**.

---

## ⚠️ Disclaimer

This project is intended **for development and testing purposes only** — such as testing location-aware features in your own iOS apps. Do not use it to misrepresent your location in apps or services in violation of their Terms of Service.

---

## 📁 Project Structure

```
LocationSnhika/
├── newlocation.gpx   # GPX file with spoofed coordinates
└── README.md         # You're reading it
```

---

## 🪪 License

MIT License — free to use and modify.
