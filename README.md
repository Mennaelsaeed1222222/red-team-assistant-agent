 Recon Agent – Passive OSINT Recon Tool

 What it does
- Performs passive reconnaissance for a single domain (no active scanning, no exploitation, no internet crawling beyond public services).
- Fast, local, and easy-to-read output suitable for developers, security students, and defenders.

 Key checks / features
- WHOIS lookup for domain registration metadata.
- Passive subdomain enumeration via `crt.sh` (certificates transparency).
- DNS resolution of discovered subdomains (A records).
- Saves results as timestamped JSON in a `results/` folder.
- Designed to be minimal-dependency and easy to run (works from a script or Jupyter cell).

 Requirements
- Python 3.8+  
- Internet connection (for crt.sh / WHOIS / DNS queries)  
- Optional: virtual environment for cleaner dependency management

 How to run (example)
1. Pick a domain you own or have explicit permission to test.
2. Run the agent from the project root:

```bash
python agent/main.py example.com
