



# NRAM

**NRAM** is a modular network auditing and brute-force tool that allows sequential execution of various scanning and brute-forcing modules. It provides real-time status updates via a web-based UI, making it easy to monitor the progress of each task. This tool is designed to target common network services such as FTP, SSH, RDP, SMB, and others, with each module handling its own scanning and attack logic.

File Structure: (for now)
NRAM/
  modules/
    ftp.py
    rdp.py
    ssh.py
    smb.py
    telnet.py
    http.py
    dns.py
    smtp.py
    pop3.py
    imap.py
    snmp.py
    mysql.py
    postgres.py
    mongodb.py
    redis.py
    utils.py
  assets/
    wordlist.txt
  data/
    scan_results.json
    brute_force_results.json
  config/
    settings.yaml
  webapp/
    static/
      css/
        style.css
      js/
        script.js
    templates/
      index.html
      results.html
    files/
      webapp.py
  root_files/
    multitool.py
    README.md
    requirements.txt


## Features
- **Modular Design**: Each module (FTP, SSH, RDP, SMB, etc.) is self-contained, handling its own scanning and brute-force logic.
- **Sequential Execution**: Runs modules in sequence to prevent resource conflicts and provide clear, ordered output.
- **Web-Based Status Dashboard**: Displays the current status of the multitool via a simple web interface.
- **Easy to Extend**: Add new modules for different network services by following the simple structure of existing modules.
- **Dynamic UI Updates**: Real-time updates to the web UI as each module progresses.

## Supported Modules
- FTP Scanning & Brute-Forcing
- SSH Scanning & Brute-Forcing
- RDP Scanning & Brute-Forcing
- SMB Scanning & Brute-Forcing
- More services to be added (Telnet, HTTP, DNS, etc.)

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/multitool.git
   cd multitool
   ```

2. **Install Dependencies**:
   Make sure Python 3 and pip are installed, then install the necessary dependencies:
   ```bash
   pip install Flask
   ```

3. **Run the Web Interface**:
   In one terminal window, start the Flask web server:
   ```bash
   cd webapp
   python webapp.py
   ```

4. **Run the Multitool**:
   In another terminal window, start the main multitool script:
   ```bash
   python multitool.py
   ```

5. **Access the Dashboard**:
   Open a web browser and visit:
   ```
   http://127.0.0.1:5000
   ```
   You will see real-time updates as the tool executes the modules.

## Usage
Multitool will execute each module in sequence, updating the web UI with the current status. Modules can be expanded or customized as needed.

### Example Modules:
- **FTP**: Scans for FTP servers and performs brute-force login attempts.
- **SSH**: Scans for SSH servers and attempts brute-force logins.
- **RDP**: Scans for RDP servers and tries to brute-force logins.
- **SMB**: Scans for SMB servers and performs login attempts.

## Future Enhancements
- Additional modules for Telnet, HTTP, DNS, etc.
- Improved vulnerability scanning and reporting.
- More configurable UI options for better status tracking.
- Integration with other tools for in-depth auditing.

## Contributing
Feel free to contribute to the project by creating new modules or improving existing functionality. Fork the repo, create a new branch, and submit a pull request with your improvements.



---
