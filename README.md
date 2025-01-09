
# 🐬 FlipperZero-BadUSB-Scripts

A collection of BadUSB scripts for Flipper Zero, including useful utilities and demonstrations of the device's capabilities. These scripts are designed for security testing and task automation.

---

## 📋 Scripts in the Repository

### 1. **System Info & Keylogger via Telegram**
- **Description:** This script collects system information (e.g., PC name, IP addresses, Wi-Fi details, and hardware information) and records keystrokes (keylogger). The data is sent to Telegram via webhooks.
- **Target Platform:** Windows
- **Features:**
  - System information collection.
  - Keylogger.
  - Data transmission to Telegram.

---

## 🚀 Step-by-Step Usage Guide

### 1. **Download the Script File**
1. Navigate to the folder corresponding to the desired script (e.g., `System Info & Keylogger`).
2. Download the PowerShell script file inside that folder (e.g., `main_script.txt`).

### 2. **Create a Telegram Bot**
1. Open Telegram and search for [@BotFather](https://t.me/BotFather).
2. Send the `/newbot` command and follow the instructions.
3. Obtain your bot's token (e.g., `123456789:ABCdefGHIjklMNOpqrstUVWXyz`).
4. Save the token for the next steps.

### 3. **Get Your Chat ID**
1. Find your bot in Telegram and start a chat with it.
2. Use the API method:
   - Open the link: `https://api.telegram.org/bot<Your_Token>/getUpdates` (replace `<Your_Token>` with your bot's token).
   - Locate the `chat` field and save the `id` value (e.g., `123456789`).

### 4. **Configure the Script**
- Open the file `main_script.txt`.
- Replace the following lines with your data:
  ```powershell
  $telegramToken = "<TOKEN>"  # Replace <TOKEN> with your bot's token
  $chatId = "<CHAT_ID>"       # Replace <CHAT_ID> with your Chat ID
  ```
- Save the changes.

### 5. **Upload the Script to Dropbox**
   - Create an account or log in to [Dropbox](https://www.dropbox.com).
   - Upload the script file to your Dropbox.
   - Get a shareable link to the uploaded file.

### 6. **Create a Short Link with Bitly**
   - Go to [Bitly](https://bitly.com) and create an account if you don't have one.
   - Paste the Dropbox link and create a short link.
   - Copy the short link (e.g., `https://bit.ly/example`).

### 7. **Edit the Ducky Script**
   - In the `System Info & Keylogger via telegram.txt` file, replace the existing link `https://bit.ly/example` with your new short link.

### 8. **Upload the Ducky Script to Flipper Zero**
   - Copy the `.txt` file to the `badusb` folder on your Flipper Zero.
   - Connect Flipper Zero to the target system and run the script.

---

## ⚠️ Important

- Use these scripts **only for legal and ethical purposes**.
- Do not use them for unauthorized access or malicious intent.
- Ensure that the Telegram token and Chat ID in the script match your settings.
- Scripts will stop working after closing PowerShell or shutting down/restarting the computer.

---

## 📄 License

This project is distributed under the [MIT License](LICENSE).

---

## 📞 Feedback

If you have any suggestions or questions, please create an [Issue](https://github.com/k1y0miiii/FlipperZero-BadUSB-Scripts/issues).
