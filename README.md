# BlackArch Tools Encyclopedia

**By [Cysec Don](https://github.com/cysec-don)**

A comprehensive, searchable encyclopedia of **all 3,235+ security tools** available in the BlackArch Linux repository, organized across **34 categories** — complete with an interactive web-based search interface, a machine-readable JSON database, and a 9-volume PDF book series.

---

## Live Web Search Interface

**Access the interactive tool search page directly in your browser:**

### https://cysec-don.github.io/Black-Arch-Tools/

This is a fully self-contained, single-page HTML application hosted on GitHub Pages. It requires no installation, no server, and no dependencies. All 3,235 tool entries are embedded directly into the page — simply load it and start searching. The page works entirely client-side with zero external API calls, meaning it functions even after the initial load if you go offline.

#### How to Use the Search Page

1. **Open the link** above in any modern web browser (Chrome, Firefox, Safari, Edge)
2. **Type a tool name** in the search bar — for example, type `sqlmap`, `nmap`, `aircrack`, or `frida` and results appear instantly as you type
3. **Filter by category** — click any of the 34 category pill buttons below the search bar to narrow results to a specific domain (e.g., "Webapp", "Scanner", "Recon", "Cracker", "Wireless")
4. **Click any tool card** to open a detailed modal with the full description, internal mechanisms, usage scenarios, example commands, strengths, weaknesses, and comparisons with similar tools
5. **Press `ESC`** or click the `×` button to close the detail modal and return to search results
6. **Combine search + filter** — type a keyword while a category filter is active to search within that category only

The search matches against tool names, category names, and description text simultaneously, so you can find tools even if you only know what they do, not what they're called. For example, searching "bluetooth" will surface every tool in the Bluetooth category plus any tool from other categories that mentions Bluetooth in its description.

---

## Features

### Search & Discovery
- **3,235+ tools** cataloged with descriptions covering every tool in the BlackArch Linux repository
- **34 categories** from the largest (Webapp with 260 tools) to the most specialized (Miscellaneous with 20 tools)
- **Real-time search** — instant filtering as you type with no server round-trips; all data is embedded in the page
- **Category filters** — 34 clickable filter buttons with tool counts, allowing you to narrow down to any single BlackArch category
- **Combined search + filter** — use both simultaneously for precision (e.g., search "sql" within the Webapp category)
- **Load-more pagination** — initially shows 100 results for performance, with a single click to expand the full list

### Tool Detail View
- **70 deep-dive entries** with comprehensive analysis including:
  - **How It Works** — internal mechanisms, algorithms, and technical architecture explained in depth
  - **Usage Scenarios** — real-world situations where the tool is applicable, from penetration tests to red team engagements
  - **Example Commands** — copy-ready terminal commands demonstrating common usage patterns
  - **Strengths** — what the tool does better than alternatives and why professionals choose it
  - **Weaknesses** — known limitations, noise levels, false positive rates, and compatibility issues
  - **Comparison with Similar Tools** — head-to-head analysis against competing tools in the same domain
- **3,165 standard entries** with category-based descriptions and installation commands
- **Installation command** for every tool (`pacman -S <toolname>`) shown in the detail modal

### Design & Performance
- **Dark theme** — designed for extended use during late-night security research and penetration testing sessions
- **Fully responsive** — works on desktop monitors, laptops, tablets, and mobile phones
- **Zero external dependencies at runtime** — all 3,235 tool entries are embedded in the HTML; no JSON fetch, no CORS issues, no API calls
- **Offline-capable** — after the first page load, the entire encyclopedia works without an internet connection
- **Keyboard-friendly** — `ESC` to close modals, `Tab` to navigate, full keyboard accessibility
- **Smooth animations** — modal slide-in effects, hover transitions, and focus indicators

---

## All 34 BlackArch Categories

The BlackArch repository organizes its 2,800+ tools into 34 distinct categories. This encyclopedia expands the catalog to 3,235 entries by including sub-tools, variants, and utility packages within each category. Below is the complete list of categories with their tool counts and descriptions:

| # | Category | Tools | Description |
|---|----------|-------|-------------|
| 1 | **Webapp** | 260 | Web application security testing — SQL injection, XSS, CSRF, directory brute-forcing, CMS scanning, API fuzzing, WAF detection and bypass |
| 2 | **Scanner** | 234 | Network and vulnerability scanning — port scanning, service detection, OS fingerprinting, vulnerability assessment, asset discovery |
| 3 | **Recon** | 223 | Reconnaissance and OSINT — subdomain enumeration, email harvesting, social media intelligence, DNS reconnaissance, certificate transparency |
| 4 | **Exploitation** | 164 | Exploit development and execution — framework exploitation, shellcode generation, ROP chains, CVE-specific exploits, post-exploitation |
| 5 | **Cracker** | 180 | Password cracking and brute-forcing — hash cracking, online brute-force, rainbow tables, wordlist generation, rule-based attacks |
| 6 | **Wireless** | 126 | Wireless network attacks — WiFi cracking, WPA/WEP attacks, evil twin setup, wireless injection, Bluetooth exploitation |
| 7 | **Forensic** | 129 | Digital forensics — disk imaging, file recovery, memory analysis, timeline reconstruction, registry parsing, evidence collection |
| 8 | **Crypto** | 128 | Cryptography tools — encryption/decryption, hash analysis, SSL/TLS auditing, steganography, key extraction, cipher identification |
| 9 | **Fuzzer** | 137 | Fuzzing frameworks — AFL and variants, protocol fuzzing, web fuzzing, grammar-based fuzzing, coverage-guided mutation |
| 10 | **Social** | 118 | Social engineering — phishing frameworks, credential harvesting, campaign management, template engines, tracking beacons |
| 11 | **Windows** | 118 | Windows/Active Directory — credential dumping, Kerberos attacks, lateral movement, C2 frameworks, privilege escalation, AD enumeration |
| 12 | **Reversing** | 92 | Reverse engineering — disassemblers, decompilers, binary analysis frameworks, SMT solvers, firmware extraction, debugging |
| 13 | **Malware** | 106 | Malware analysis — sandboxing, YARA rules, PE analysis, unpacking, obfuscation detection, threat intelligence, IOC extraction |
| 14 | **Backdoor** | 89 | Backdoor tools — reverse shells, bind shells, web shells, persistent access, DNS tunneling, C2 communication |
| 15 | **Mobile** | 97 | Mobile security — Android/iOS analysis, APK decompilation, Frida instrumentation, mobile forensics, jailbreak tools |
| 16 | **Sniffer** | 77 | Network sniffing — packet capture, traffic analysis, MITM attacks, protocol dissection, intrusion detection |
| 17 | **Networking** | 110 | Network utilities — tunneling, proxying, VPN, DNS tools, file transfer, SSH, remote access, network configuration |
| 18 | **Defensive** | 86 | Defensive security — IDS/IPS, SIEM, HIDS, log analysis, threat intelligence feeds, intrusion detection, file integrity monitoring |
| 19 | **Bluetooth** | 79 | Bluetooth security — BLE sniffing, device enumeration, pairing attacks, Bluetooth honeypots, SDR integration |
| 20 | **Proxy** | 64 | Proxy tools — intercepting proxies, SOCKS/HTTP proxying, traffic manipulation, chain proxying, anonymization |
| 21 | **Tunnel** | 58 | Tunneling tools — DNS tunneling, HTTP tunneling, ICMP tunneling, SSH tunneling, covert channels |
| 22 | **Spoof** | 59 | Spoofing tools — ARP spoofing, DNS spoofing, DHCP spoofing, MITM via spoofing, credential interception |
| 23 | **Dos** | 63 | Denial of Service — stress testing, rate limiting tests, protocol-level DoS, application-layer DoS, slowloris variants |
| 24 | **Radio** | 66 | Software-defined radio — SDR tools, signal analysis, RF monitoring, GSM analysis, GPS spoofing, satellite communication |
| 25 | **VoIP** | 50 | Voice over IP — SIP scanning, VoIP eavesdropping, VoIP fuzzing, PBX attacks, call interception |
| 26 | **Stego** | 50 | Steganography — hidden data detection, image/audio steganography, LSB encoding, watermark extraction, stego analysis |
| 27 | **Binary** | 51 | Binary analysis — ELF/PE parsing, binary diffing, symbol analysis, patch management, binary signing |
| 28 | **Code Audit** | 49 | Source code auditing — static analysis, dependency scanning, vulnerability pattern detection, SAST tools |
| 29 | **Automation** | 45 | Security automation — workflow engines, pipeline integration, batch scanning, report generation, CI/CD security |
| 30 | **Honeypot** | 36 | Honeypot deployment — SSH honeypots, web honeypots, DNS honeypots, attack attribution, deception technology |
| 31 | **Packer** | 23 | Executable packing — UPX variants, custom packers, compression, anti-debugging, anti-disassembly |
| 32 | **Debugger** | 27 | Debugging tools — GDB extensions, dynamic analysis, breakpoint management, memory inspection, runtime hooking |
| 33 | **Disassembler** | 21 | Disassembly engines — Capstone, objdump variants, instruction decoding, control flow analysis |
| 34 | **Misc** | 20 | Miscellaneous — uncategorized tools, utilities, and specialized instruments that don't fit other categories |

---

## Book Series: BlackArch Linux — The Definitive Arsenal

The `pdfs/` directory contains the complete 9-volume book series authored by **Cysec Don**, providing exhaustive coverage of every tool in the BlackArch repository. This is not a summary or overview — each volume dissects every tool in its category with the following structure:

### 7-Part Book Structure

| Part | Content |
|------|---------|
| **Part 1: Foundations** | BlackArch architecture, design philosophy, the 48 categories explained, installation methods (ISO, repository overlay, slim ISO), system configuration |
| **Part 2: Category-by-Category Breakdown** | Every tool examined individually with deep description, internal mechanisms, usage scenarios, example commands, strengths, weaknesses, and comparisons |
| **Part 3: Tool Relationships** | How tools connect and complement each other, pipeline compositions, tool chaining strategies, when to use which combination |
| **Part 4: Advanced Usage** | Expert-level configurations, custom scripting, automation, integration with CI/CD pipelines, performance tuning |
| **Part 5: Real-World Attack Simulations** | Complete attack chains using multiple BlackArch tools, red team scenarios, APT emulation, purple team exercises |
| **Part 6: Defensive Perspective** | How defenders detect and counter each tool, defensive recommendations, hardening strategies, monitoring and alerting |
| **Part 7: Lab Environment** | Setting up practice environments, vulnerable VMs, CTF challenges, safe experimentation setups, legal considerations |

### Volume Breakdown

| Volume | Title | Pages | Focus |
|--------|-------|-------|-------|
| Vol 1 | Foundations & WebApp Tools | ~100+ | BlackArch architecture, category system, installation guide, then exhaustive coverage of all 260+ web application security tools including SQLMap, Nikto, Gobuster, WPScan, Burp Suite, OWASP ZAP, ffuf, and 253 more |
| Vol 2 | Scanner Tools | ~80+ | 234 scanning and enumeration tools — Nmap, Masscan, RustScan, OpenVAS, Nessus, Zgrab2, and every other scanner from ARP discovery to vulnerability assessment |
| Vol 3 | Recon & Exploitation | ~120+ | 223 reconnaissance tools (Amass, Subfinder, Maltego, SpiderFoot, Recon-ng, Shodan, Censys) plus 164 exploitation tools (Metasploit, BeEF, ExploitDB, pwntools, ROP chains, CVE-specific exploits) |
| Vol 4 | Cracker & Wireless | ~90+ | 180 password cracking tools (John the Ripper, Hashcat, Hydra, Medusa, Ncrack) plus 126 wireless attack tools (Aircrack-ng, Wifite, Kismet, Reaver, EAPHammer, Fluxion) |
| Vol 5 | Forensic, Crypto & Fuzzer | ~100+ | 129 forensic tools (Autopsy, Sleuth Kit, Volatility), 128 crypto tools (OpenSSL, GPG, Steghide, Ciphey), and 137 fuzzing tools (AFL++, Honggfuzz, LibFuzzer, Boofuzz) |
| Vol 6 | Social, Windows, Reversing & Malware | ~120+ | 118 social engineering tools (SET, GoPhish, Evilginx2), 118 Windows/AD tools (Mimikatz, BloodHound, CrackMapExec), 92 reversing tools (Ghidra, IDA, Radare2), 106 malware tools (YARA, Cuckoo, CAPE) |
| Vol 7 | Backdoor, Mobile, Sniffer, Networking & Defensive | ~130+ | 89 backdoor tools, 97 mobile security tools (Frida, Objection, Drozer, APKTool), 77 sniffer tools (Wireshark, Bettercap), 110 networking tools, 86 defensive tools (Wazuh, Suricata, Zeek) |
| Vol 8 | Specialized Categories | ~200+ | Bluetooth (79 tools), Proxy (64), Tunnel (58), Spoofing (59), DoS (63), Radio/SDR (66), VoIP (50), Steganography (50), Binary (51), Code Audit (49), Automation (45), Honeypot (36), Packer (23), Debugger (27), Disassembler (21), Misc (20) |
| Vol 9 | Advanced Topics | ~60+ | Tool relationship mapping, advanced multi-tool compositions, complete attack simulation walkthroughs, defensive countermeasures for every tool category, lab environment setup guides |

---

## Quick Start

### Option 1: Use the Live Web Interface (Recommended)

Simply open this URL in any browser:

**https://cysec-don.github.io/Black-Arch-Tools/**

No installation required. Works on any device with a modern web browser.

### Option 2: Run Locally

```bash
# Clone the repository
git clone https://github.com/cysec-don/Black-Arch-Tools.git
cd Black-Arch-Tools

# Open the HTML file in your default browser
# On Linux:
xdg-open index.html

# On macOS:
open index.html

# On Windows:
start index.html

# Or simply double-click index.html in your file manager
```

### Option 3: Use the JSON Data Programmatically

The `tools_full.json` file contains the complete tool database in a machine-readable format, suitable for integration into your own scripts, tools, or applications:

```python
import json

# Load the tool database
with open('tools_full.json', 'r') as f:
    tools = json.load(f)

# Find all tools in the wireless category
wireless_tools = [t for t in tools if t['category'] == 'blackarch-wireless']
print(f"Wireless tools: {len(wireless_tools)}")

# Find tools with detailed analysis
detailed = [t for t in tools if t.get('detailed')]
print(f"Deep-dive entries: {len(detailed)}")

# Search for SQL-related tools
sql_tools = [t for t in tools if 'sql' in t['description'].lower() or 'sql' in t['name'].lower()]
for tool in sql_tools:
    print(f"  {tool['name']} ({tool['category_display']})")
```

### Option 4: Install BlackArch Tools

If you want to install any of the cataloged tools on an Arch Linux system:

```bash
# Add the BlackArch repository (one-time setup)
curl -O https://blackarch.org/strap.sh
chmod +x strap.sh
sudo ./strap.sh

# Install a specific tool
sudo pacman -S sqlmap

# Install all tools in a category
sudo pacman -S blackarch-webapp

# Install the entire BlackArch collection (50+ GB)
sudo pacman -S blackarch
```

---

## Data Format

The `tools_full.json` file contains the complete tool database. Each entry follows this schema:

### Detailed Tool Entry (70 tools)

```json
{
  "name": "sqlmap",
  "category": "blackarch-webapp",
  "category_display": "Webapp",
  "description": "SQLMap is the gold standard for automated SQL injection detection and exploitation...",
  "how_it_works": "SQLMap works by sending crafted HTTP requests with SQL payload variations to the target parameter. It uses a technique called 'boolean-based blind'...",
  "usage_scenarios": "Testing web applications for SQL injection during penetration tests. Extracting credentials...",
  "commands": [
    "sqlmap -u 'http://target/page?id=1' --dbs",
    "sqlmap -u 'http://target/page?id=1' -D dbname --tables",
    "sqlmap -u 'http://target/page?id=1' -D dbname -T users --dump",
    "sqlmap -u 'http://target/page?id=1' --os-shell",
    "sqlmap -r request.txt --batch --level=5 --risk=3"
  ],
  "strengths": [
    "Supports all 6 SQL injection techniques automatically",
    "Can escalate from data extraction to OS shell",
    "Massive database of injection payloads and tamper scripts",
    "Session resumption and batch mode for automation"
  ],
  "weaknesses": [
    "Noisy - generates thousands of requests that WAFs can detect",
    "Can crash databases with aggressive settings (--risk=3)",
    "False positives on complex applications with non-standard responses",
    "Steep learning curve for advanced features and tamper scripts"
  ],
  "comparison": "jSQL Injection offers a GUI alternative but lacks SQLMap's depth and technique coverage. NoSQLMap targets NoSQL databases...",
  "detailed": true
}
```

### Standard Tool Entry (3,165 tools)

```json
{
  "name": "feroxbuster",
  "category": "blackarch-webapp",
  "category_display": "Webapp",
  "description": "A webapp-category security tool available in the BlackArch Linux repository...",
  "detailed": false
}
```

### Field Reference

| Field | Type | Always Present | Description |
|-------|------|---------------|-------------|
| `name` | string | Yes | The tool's package name (used for `pacman -S <name>`) |
| `category` | string | Yes | The BlackArch category key (e.g., `blackarch-webapp`) |
| `category_display` | string | Yes | Human-readable category name (e.g., `Webapp`) |
| `description` | string | Yes | Full description of the tool's purpose and capabilities |
| `how_it_works` | string | Detailed only | Technical explanation of internal mechanisms and architecture |
| `usage_scenarios` | string | Detailed only | Real-world situations where the tool is applicable |
| `commands` | array | Detailed only | List of example terminal commands |
| `strengths` | array | Detailed only | List of the tool's key advantages |
| `weaknesses` | array | Detailed only | List of the tool's known limitations |
| `comparison` | string | Detailed only | Analysis comparing against similar/competing tools |
| `detailed` | boolean | Yes | `true` for the 70 deep-dive entries, `false` for standard entries |

---

## Repository Structure

```
Black-Arch-Tools/
├── index.html              # Self-contained interactive search page (1 MB)
│                           # - All 3,235 tools embedded as JavaScript
│                           # - Zero external API calls
│                           # - Works offline after first load
│                           # - Dark theme, responsive, keyboard-friendly
│
├── tools_full.json         # Complete tool database (1 MB)
│                           # - Machine-readable JSON array
│                           # - 70 detailed entries + 3,165 standard entries
│                           # - Suitable for programmatic use
│
├── README.md               # This documentation file
│
└── pdfs/                   # 9-volume PDF book series
    ├── BlackArch_Vol1_Foundations_WebApp.pdf          (~960 KB)
    ├── BlackArch_Vol2_Scanner_Tools.pdf               (~960 KB)
    ├── BlackArch_Vol3_Recon_Exploitation.pdf           (~1.3 MB)
    ├── BlackArch_Vol4_Cracker_Wireless.pdf             (~960 KB)
    ├── BlackArch_Vol5_Forensic_Crypto_Fuzzer.pdf       (~1.2 MB)
    ├── BlackArch_Vol6_Social_Windows_Reversing_Malware.pdf (~1.3 MB)
    ├── BlackArch_Vol7_Backdoor_Mobile_Sniffer_Net_Defend.pdf (~1.4 MB)
    ├── BlackArch_Vol8_Specialized_Categories.pdf       (~2.2 MB)
    └── BlackArch_Vol9_Advanced_Topics.pdf              (~80 KB)
```

---

## Technical Details

### How the Search Page Works

The `index.html` file is a fully self-contained single-page application. On page load, it initializes a JavaScript array (`TOOLS`) containing all 3,235 tool entries embedded directly in the HTML source. The search and filter logic runs entirely in the browser:

1. **Search** — the input handler fires on every keystroke with a 150ms debounce, filtering the `TOOLS` array against the query string by matching against `name`, `category_display`, and `description` fields (case-insensitive)
2. **Category filters** — clicking a filter button sets the `activeFilter` variable and re-runs the filter pipeline, combining with any active search query
3. **Rendering** — the first 100 matching tools are rendered as DOM cards for performance; a "load more" button appears if there are additional results
4. **Detail modal** — clicking a card opens a modal overlay with the full tool information; the modal slides in with a CSS animation and closes on `ESC`, `×` click, or overlay click
5. **No external requests** — the page makes zero network requests after the initial load (Google Fonts are optional and gracefully degrade to system fonts)

### Browser Compatibility

| Browser | Supported | Notes |
|---------|-----------|-------|
| Chrome 80+ | Yes | Fully supported |
| Firefox 78+ | Yes | Fully supported |
| Safari 14+ | Yes | Fully supported |
| Edge 80+ | Yes | Chromium-based, fully supported |
| Mobile Safari | Yes | Responsive layout adapts to phone screens |
| Mobile Chrome | Yes | Responsive layout adapts to phone screens |
| IE 11 | No | Not supported (uses modern CSS and ES6) |

---

## Contributing

This is a living document. If you find errors, missing tools, or have improvements to suggest:

1. **Open an Issue** at [github.com/cysec-don/Black-Arch-Tools/issues](https://github.com/cysec-don/Black-Arch-Tools/issues)
2. **Submit a Pull Request** with corrections or additions to the tool database
3. **Request a detailed entry** — if you want a specific tool upgraded from a standard entry to a deep-dive analysis, open an issue with the tool name

Priority areas for contributions:
- Expanding the 70 detailed entries to cover more tools
- Correcting tool descriptions and category assignments
- Adding missing example commands for standard entries
- Reporting tools that have been added to or removed from the BlackArch repository

---

## Author

**Cysec Don**

- GitHub: [https://github.com/cysec-don](https://github.com/cysec-don)
- Repository: [https://github.com/cysec-don/Black-Arch-Tools](https://github.com/cysec-don/Black-Arch-Tools)
- Live Search: [https://cysec-don.github.io/Black-Arch-Tools/](https://cysec-don.github.io/Black-Arch-Tools/)

---

## License

This project is provided for educational and security research purposes. All tools described are part of the [BlackArch Linux](https://blackarch.org/) open-source repository. The documentation, search interface, and book series are original works by Cysec Don.

**Disclaimer:** The tools documented in this encyclopedia are powerful security instruments that should only be used on systems you own or have explicit written authorization to test. Unauthorized access to computer systems is illegal in most jurisdictions. The author assumes no liability for misuse of this information.

---

*BlackArch Linux: The Definitive Arsenal — Because knowing your tools is the first step to mastering them.*
