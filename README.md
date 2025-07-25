ChatGPT said:
markdown

# subdomain-passive-info

A simple Bash tool for passive reconnaissance on a target domain. It gathers WHOIS data, runs basic string filtering, performs a DMITRY scan, and enumerates subdomains using Assetfinder and Subfinder.

---

## Features

- **WHOIS Lookup**: Collect domain registration details  
- **Quick grep**: Extract numeric and common patterns from WHOIS output  
- **Passive Scan**: Use [DMITRY](https://github.com/jondufresne/dmitry) for email, netcraft, subdomains, ports, and more  
- **Subdomain Enumeration**: Consolidate results from [Assetfinder](https://github.com/tomnomnom/assetfinder) and [Subfinder](https://github.com/projectdiscovery/subfinder)

---

## Installation

1. Clone the repo:  
   ```bash
   git clone https://github.com/anjalijaglan07/subdomain-passive-info.git
   cd subdomain-passive-info
2. Make the script executable:
   ```bash
   chmod +x subdomain-passive-info.sh

---

## Usage
Run the script and follow the prompts:
```bash
./subdomain-passive-info.sh
```
1. Enter your target domain (e.g. `example.com`)
2. Choose scan type:

-`p` → Passive information gathering (DMITRY)

-`sb` → Subdomain enumeration (Assetfinder + Subfinder)

3. Outputs will be saved as:

-`whois.txt`

-`assetfinder.txt`

-`subfinder.txt`

-`subdomain-output.txt`

---

## Prerequisites
Ensure the following tools are installed and available in your $`PATH`:
```bash
# Debian/Ubuntu
sudo apt update && sudo apt install -y whois dmitry

# Go-based tools (ensure Go is installed)
go install github.com/tomnomnom/assetfinder@latest
go install github.com/projectdiscovery/subfinder/v2/cmd/subfinder@latest
```
---
## File Structure
```
subdomain-passive-info/
├── subdomain-passive-info.sh  
├── README.md

```
---

## Contact

**Anjali Jaglan**  
B.Tech in Cyber-Security, PIET Panipat  
LinkedIn: [anjali-jaglan-3968b8248](https://www.linkedin.com/in/anjali-jaglan-3968b8248)  
GitHub: [anjali-jaglan07](https://github.com/anjalijaglan07)  

