# 🌱 SEEDS (ProjectZero)

**SEEDS** is a lightweight, zero-config tool for ultra-fast file sharing between devices within the same local network. No internet, no cloud, no registration — just direct peer-to-peer transfer.

### ⚡ Features

- **Instant Start:** Run the executable and your server is live.
    
- **Cross-Platform:** Seamlessly transfer files between Windows, Linux, Android, and iOS via any web browser.
    
- **Auto-Cleanup:** Privacy first. The `downloads` folder is automatically purged every time the server starts.
    
- **Live Monitoring:** See exactly who is connected to your session with the real-time "Active Devices" list.
    
- **Smart IP Detection:** Automatically identifies your correct local network address, skipping useless virtual or APIPA (169.254.x.x) IPs.
    

---

## 📥 Installation & Setup

Currently, **SEEDS** is distributed as pre-compiled binaries:

1. **Download** the version for your OS from the [Releases](https://www.google.com/search?q=https://github.com/your-username/seeds/releases) section.
    
    - `seeds.exe` (Windows)
        
    - `seeds` (Linux/macOS)
        
2. **Run the application:**
    
    - **Windows:** Double-click the file.
        
    - **Linux:** Open terminal, run `chmod +x seeds` and then `./seeds`.
        
3. **Access the Dashboard:** The program will display a local URL (e.g., `http://192.168.1.15:44069`). Simply type this address into the browser of any other device on the same Wi-Fi.
    

---

## ⚠️ Important Note for Windows Users

When running **SEEDS**, you might encounter **Windows SmartScreen** or **Defender** warnings:

- **Why?** The app is written in Go and is not digitally signed with a costly corporate certificate. Windows often flags unsigned `.exe` files as "unknown" or "suspicious."
    
- **Is it safe?** Yes. This is a local-only tool.
    
- **How to bypass:** 1. Click **"More info"**. 2. Click **"Run anyway"**. 3. If the **Firewall** prompt appears, select **"Allow access"** for Private Networks, otherwise other devices won't be able to find your PC.
    

---

## 🚀 How to Use

1. **Host the Server:** Start the app on your main PC.
    
2. **Connect:** Copy the displayed URL or use the QR code (if available) to open the interface on your phone or another laptop.
    
3. **Upload:** Use the "Upload" button to send files to the host PC. They will appear in the `./downloads` folder.
    
4. **Share:** Place any files you want to distribute into the `./shared` folder next to the app. They will instantly appear for everyone connected.
    

---

## 🛠 Tech Stack

- **Backend:** Go (Golang) — for high-performance networking.
    
- **Frontend:** Vanilla JS / CSS (Dark Purple / Cyberpunk Aesthetic).
    
- **Security:** Built-in connection tracker & session-based file isolation.
    

---

> **Note:** Source code is currently private and will be released at a later stage. Stay tuned for updates!
