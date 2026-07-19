# THOOL

THOOL is a Python-based enumeration tool for reconnaissance and security testing. The name is a combination of **"the"** and **"tool"**, making it simple and memorable.

> **Note:** THOOL is currently in **beta**. New features, improvements, and bug fixes will be added over time.

## Features

* Directory enumeration
* Subdomain enumeration
* Port scanning
* Easy-to-use command-line interface

---

# Installation

## Requirements

* Python 3.10+
* `pip`

Install the required dependencies:

```bash
pip install -r requirements.txt
```

---

# Add THOOL to your PATH

This allows you to run `thool` from any directory.

## macOS

Open your shell configuration:

```bash
nano ~/.zshrc
```

Make it executable

```bash
chmod +x thool
```

Add the following line at the end of the file:

```bash
export PATH="$PATH:/path/to/thool"
```

Save the file:

* **Ctrl + O**, then **Enter**
* **Ctrl + X** to exit

Reload your shell:

```bash
source ~/.zshrc
```

## Linux

Move the executable to `/usr/local/bin`:

```bash
sudo cp thool /usr/local/bin/
sudo chmod +x /usr/local/bin/thool
```

Verify the installation:

```bash
thool -h
```

---

# Usage

Display the help menu:

```bash
thool -h
```

```
usage: thool [-h] [-u URL] [-t TARGET] [-dir] [-sub] [-port] [-a] [-w WORDLIST]

Enumerating Target Domain

options:
  -h, --help                 Show this help message and exit
  -u, --url URL              Target URL (example.com or https://example.com)
  -t, --target TARGET        Target IP address
  -dir, --directory_enum     Enable directory enumeration
  -sub, --subdomain_enum     Enable subdomain enumeration
  -port, --port_scanning     Enable port scanning | Either TCP or UDP with -p tcp and -p udp
  -a, --every_script         Run all available enumeration modules
  -w, --wordlist PATH        Path to wordlist
```

---

# Examples

### Directory Enumeration

```bash
thool -u example.com -dir -w wordlist.txt
```

### Subdomain Enumeration

```bash
thool -u example.com -sub -w wordlist.txt
```

### Port Scan

```bash
thool -t 192.168.0.10 -p tcp
```

### Run All Modules

```bash
thool -u example.com -t 192.168.0.10 -a -w wordlist.txt
```

---

# Disclaimer

THOOL is intended for **educational purposes** and **authorized security testing only**.

Only use this tool against systems that you own or have explicit permission to test. Unauthorized scanning or enumeration of third-party systems may violate laws, regulations, or acceptable use policies.

---

# License

This project is open source. Feel free to contribute by submitting issues or pull requests.
