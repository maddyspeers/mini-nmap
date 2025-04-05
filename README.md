# 🕵️‍♂️ Mini-Nmap: Vulnerability Scanner

A simplified port scanner written in Python that scans a target IP address for open ports and flags risky services (like Telnet, FTP, etc.). Inspired by Nmap!

## 🚀 Features

- Scan for open TCP ports on any host (including localhost)
- Identify and flag insecure services (e.g., Telnet, FTP)
- Clear CLI output with port status and risk indicators
- Lightweight — uses only Python sockets 

## 🔧 Technologies Used

- Python 3.x
- `socket` module (required)

## 📦 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/maddyspeers/mini-nmap.git
   cd mini-nmap
2. Run the script:
    ```bash
   python scanner.py

## 🖥 Example output
Scanning localhost from port 20 to 100...


[OPEN] Port 22 - SSH


[OPEN] Port 8080 - HTTP


[RISK] Port 23 - Telnet (insecure protocol)



Scan complete. 3 open ports found, 1 flagged as risky.

## ⚠️ Risky Services Flagged

| Port | Service | Risk            |
|------|---------|------------------|
| 21   | FTP     | ⚠️ Unencrypted   |
| 23   | Telnet  | ⚠️ Insecure      |
| 110  | POP3    | ⚠️ Legacy Email  |
| 143  | IMAP    | ⚠️ Legacy Email  |



## 🧪 Future Ideas
- Add banner grabbing for service fingerprinting
- Enable UDP scan mode
- GUI using Tkinter or PyQt
- Export scan results to a file

## 🛡 Disclaimer
This tool is intended for educational and ethical use only. Always get permission before scanning external IP addresses.

## Made with ❤️ by me for learning and experimentation!
