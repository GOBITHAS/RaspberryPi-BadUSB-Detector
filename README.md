# RaspberryPi-BadUSB-Detector
A Raspberry Pi 5, based BadUSB Detection Tool that identifies, analyses, and blocks malicious USB devices in real time using device fingerprinting, behavioural analysis, USBGuard integration, and automated alerting.

# Raspberry Pi BadUSB Detection Tool

A hardware–software integrated security system designed to detect, analyze, and block BadUSB attacks in real time.  
Built using **Raspberry Pi 5**, **Python**, **USBGuard**, and **behavioral fingerprinting**, this tool identifies both normal and malicious USB devices and alerts users instantly.

---

## 🚀 Features

- 🛡️ Real-time USB monitoring  
- 🔍 Device fingerprinting (VID, PID, class, serial, power)  
- 👾 BadUSB attack detection (HID spoofing, re-enumeration)  
- 🚫 Automatic blocking using USBGuard  
- 📊 GUI Dashboard (Tkinter)  
- 💻 CLI Monitoring Mode  
- 📬 Email alerting system (HTML formatted)  
- 📁 Full forensic logging  
- 🧠 Behaviour-based detection rules  
- 🧪 Documented test cases & validation results  

---

📂 Project Structure

src/ – detection engine & dashboards
config/ – USBGuard + JSON configs
docs/ – final report & diagrams
diagrams/ – architecture & system flowcharts
screenshots/ – UI & alert screenshots
logs/ – generated logs


---

## 🛠️ Installation (Raspberry Pi 5)

### 1️⃣ Update Pi
sudo apt update && sudo apt upgrade -y


### 2️⃣ Install Dependencies
sudo apt install python3-pip usbguard -y
pip3 install -r requirements.txt


### 3️⃣ Start USBGuard
sudo systemctl enable usbguard
sudo systemctl start usbguard


### 4️⃣ Start Detector
python3 src/badusb_detector.py


---

## ⚙️ Configuration

### Email Alerts  
Update your email credentials inside:
config/settings.json


### USBGuard Policy  
config/usbguard.conf


---

## 🖼️ Screenshots

| GUI Dashboard | CLI Output | Email Alert |
|--------------|------------|--------------|
| ![](screenshots/gui_dashboard.png) | ![](screenshots/cli_output.png) | ![](screenshots/email_alert.png) |

---

## 🧪 Testing & Validation

The system was tested using:

- Normal USB storage devices  
- HID keyboards  
- Modified BadUSB payload devices  
- Multi-device enumeration tests  

Results:

- ✔ 100% successful detection  
- ✔ No false positives  
- ✔ 1–2 second response time  

---

## 📘 Documentation

Complete project documentation can be found in:
docs/Final_Report.pdf


---

## 📜 License
This project is licensed under the **MIT License**.

---

## 👤 Author

**Yogarasa Gobithas** 
BSc(Hons) Cybersecurity & Digital Forensics  
Kingston University London  

If you found this helpful, ⭐ star the repository!




