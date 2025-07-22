# 🔔 Click2ADS Pro – Chrome Click-to-Call Extension

**Click2ADS Pro** is a professional Chrome extension designed for call centers, sales teams, and support agents. It enables instant click-to-call functionality via WebRTC or SIP phones (e.g., Yealink), and includes advanced tools like an AutoDialer, integrated softphone, performance stats, and multi-SIP account management.

---

## 🚀 Features Included

### 🏠 Main Popup (Click2Call)
- 📲 Manual phone number input
- 🎛️ Select default SIP account
- ☎️ One-click calling through:
  - WebRTC (browser)
  - AMI → SIP Phone (e.g., Yealink)
- 🔁 Start / Stop AutoDialer
- ✅ Auto-detection of call method
- 🌐 "WebRTC Enabled" checkbox
- 🪟 Automatic opening of WebRTC softphone popup
- 📤 Saves last dialed number
- 📊 Direct access to **Statistics**
- ⚙️ Direct access to **Options**

---

### ⚙️ Options (SIP Account Management)
- ➕ Add SIP accounts via form
- 📝 Fields supported:
  - Name, Extension, Domain, Username, Password, Port
- ✅ Enable WebRTC per account
- 🌟 Set default SIP account
- 📋 Account list displayed in a responsive table
- ✏️ Edit existing accounts
- 🗑️ Delete accounts
- 🟢🔴 Status indicators:
  - SIP (Registered)
  - AMI (Connected)
  - WebSocket (WSS active)
- 🔐 Passwords hidden in UI
- ⚠️ Limit to 10 accounts for clarity and UX

---

### 📞 Integrated WebRTC Softphone (popup)
- 📡 Auto connect to WSS server
- 🧠 Auto-load current number to call
- 📞 Call / Hang up
- 🔇 Mute / Unmute
- 🎹 Toggle numeric keypad
- 🧾 Display active SIP account
- 🔁 Auto-reconnect if WebSocket drops
- ✅ Status indicators: Connected / In Call / Ended

---

### 📊 Call Statistics (stats.html)
- 🕒 View all past call logs
- 🔎 Filters:
  - Date range
  - Call status (answered, failed, voicemail…)
  - Country code / prefix
  - Used extension
- 📈 Graphs:
  - 📊 Pie chart (status)
  - 📉 Line chart (calls per day)
- 🗂️ Table with details:
  - Date, number, duration, status, extension
- ⬇️ Export to CSV
- 🖨️ Export to PDF
- ♻️ Auto-clean old logs (>1000 entries)

---

### 🔁 AutoDialer
- 🎯 Auto call list of numbers
- ⏩ Skip to next on answer or hang up
- 🧠 Includes **AMD** (Answering Machine Detection)
  - HUMAN vs MACHINE
- 🛑 Manual STOP button
- 📝 Updates call statuses automatically

---

### 🔒 Security & Local Storage
- 🔐 Uses `chrome.storage.local` for all data
- 🔒 Nothing sent externally without user consent
- 🧼 Auto-clean logs
- 🧠 Input validation on all forms
- 🛡️ SIP passwords visually encoded
- 🧩 Modular architecture – no forced server required

---

## 📁 Project Structure

click2ads-pro/
├── manifest.json  
├── popup.html / popup.js  
├── options.html / options.js  
├── stats.html / stats.js  
├── webrtc_ui.html / webrtc_ui.js  
├── dialer.js / utils.js  
├── img/ (icons 16, 48, 128 px)  
└── docs/ (User PDF Guide)  

---

## 📄 Documentation

📘 See `docs/Click2ADS-Pro-Guide.pdf` for the full illustrated guide.

---

## 🧠 Technologies Used

- JavaScript (vanilla)
- SIP.js (WebRTC)
- Chart.js (Statistics)
- Chrome Extension – Manifest V3
- FreePBX / Asterisk (via AMI)
- `chrome.storage.local` (for local persistence)

---

## 📜 License

© 2025 – Ads Media Consulting Ltd  
Commercial use only. Do not redistribute without authorization.
