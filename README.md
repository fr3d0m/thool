# THOOL
<h3>thool is a joint between the words 'the' and 'tool', which should make it easier to remember. Thool is a python file used for enumeration. This tool is only in the beta version and will be overworked by the time.</h1>

# How to set up
<p>side note: these steps can only be used on macOS and Linux.</p>
<h2>Export the path of the tool so that you can use it from any directory.</h2>
<h3>On macOS:</h3>
<h4>➜  ~ nano ~/.zshrc</h4>
<h4>Then on the last line put this:</h4>
<h4>export PATH="$PATH:/path/to/thool"</h4>
<h4>Ctrl + O, Enter to save and Ctrl + X to exit</h4>
<h3>On Linux:</h3>
<h4>move the file to /usr/local/bin/</h4>

# How to use it
```bash
(venv) ➜  ~ thool -h
 _____ _   _  ___   ___  _     
|_   _| | | |/ _ \ / _ \| |    
  | | | |_| | | | | | | | |    
  | | |  _  | |_| | |_| | |___ 
  |_| |_| |_|\___/ \___/|_____|
                               

usage: thool [-h] -u URL [-dir] [-sub] [-port] [-a] [-w WORDLIST]

Enumerating Target Domain

options:
  -h, --help            show this help message and exit
  -u, --url URL         Target URL (example.com oder https://example.com)
  -dir, --directory_scanning
                        Enable directory enumeration
  -sub, --subdomain_scanning
                        Enable subdomain enumeration
  -port, --port_scanning
                        Enable port scanning
  -a, --every_script    Run every enumeration script
  -w, --wordlist WORDLIST
                        Path to wordlist

