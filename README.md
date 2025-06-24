# Python Keylogger with Email Reporting

> ⚠️ **Disclaimer**  
> This project is intended **for educational purposes only**. Unauthorized use of keyloggers is illegal and unethical. Only run this code on systems you own or have explicit permission to test.

## 📌 Description

This Python script is a basic **keylogger** that logs keyboard input and emails the logs to a specified email address. It uses the `pynput` library for capturing keystrokes and `smtplib` to send the collected data via email.

## 🚀 Features

- Captures all keystrokes (including special keys like Enter, Tab, Backspace).
- Stores logs in a file named `keylogger.txt`.
- Sends the log file to your email automatically after the logger stops (pressing the Escape key).

## 🧰 Requirements

- Python 3.x
- `pynput` library

Install required packages using pip:

```bash
pip install pynput
````

## 🛠️ Configuration

Before running the script, update these values in the code:

```python
sender_mail = "user@domain.com"     # Your email address
receiver_mail = "user@domain.com"   # Receiver's email (can be the same)
password = "passcode"               # Your email account password
```

> ⚠️ Use an **App Password** if you're using Gmail and have 2FA enabled.

## 🏃‍♂️ Usage

1. Update the configuration with your email credentials.
2. Run the script:

```bash
python keylogger.py
```

3. The script will start logging keys. Press `Esc` to stop.
4. It will automatically email the collected logs to the configured address.

## 📂 Output

The keystrokes are saved in a file named `keylogger.txt`, which is appended to the email message.

## 📧 Email Example

```
From: user@domain.com
To: user@domain.com
Subject: KeyLogs

Text: Keylogs 
<contents of keylogger.txt>
```

## ⚠️ Legal Notice

Using keyloggers on devices you do not own or have not been authorized to monitor is **illegal**. This tool is provided solely for **educational** and **ethical testing** purposes. The developer assumes **no responsibility** for any misuse.

