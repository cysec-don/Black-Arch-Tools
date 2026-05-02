# BlackArch Tools Encyclopedia

**By [Cysec Don](https://github.com/cysec-don)**

A comprehensive, searchable encyclopedia of **all 3,235+ security tools** available in the BlackArch Linux repository, organized across **34 categories**.

## Live Search

Open `index.html` in any web browser to access the interactive tool search page. Simply type a tool name, category, or keyword to instantly find any BlackArch tool along with its description.

### Features

- **3,235+ tools** cataloged with descriptions
- **34 categories** from webapp to misc
- **70 deep-dive entries** with full analysis including:
  - How it works (internal mechanisms)
  - Usage scenarios
  - Example commands
  - Strengths and weaknesses
  - Comparison with similar tools
- **Real-time search** - instant filtering as you type
- **Category filters** - narrow down by any BlackArch category
- **Dark theme** - easy on the eyes during late-night sessions

## Book Series: BlackArch Linux - The Definitive Arsenal

The `pdfs/` directory contains the complete 9-volume book series:

| Volume | Title | Focus |
|--------|-------|-------|
| Vol 1 | Foundations & WebApp Tools | Architecture, categories, installation, 317+ webapp tools |
| Vol 2 | Scanner Tools | 309 scanning and enumeration tools |
| Vol 3 | Recon & Exploitation | 255 recon + 181 exploitation tools |
| Vol 4 | Cracker & Wireless | 161 cracker + 133 wireless tools |
| Vol 5 | Forensic, Crypto & Fuzzer | 125 forensic + 110 crypto + 103 fuzzer tools |
| Vol 6 | Social, Windows, Reversing & Malware | Social engineering, Windows AD, reverse engineering, malware analysis |
| Vol 7 | Backdoor, Mobile, Sniffer, Networking & Defensive | Backdoors, mobile security, sniffing, networking, defensive tools |
| Vol 8 | Specialized Categories | Bluetooth, proxy, tunnel, spoofing, DoS, radio, VoIP, stego, binary, code audit |
| Vol 9 | Advanced Topics | Tool relationships, advanced usage, attack simulations, defense, labs |

## Quick Start

1. Clone this repository
2. Open `index.html` in your browser
3. Search for any tool by name, category, or keyword
4. Click any tool card to see full details

## Data Format

The `tools_full.json` file contains the complete tool database:

```json
{
  "name": "sqlmap",
  "category": "blackarch-webapp",
  "category_display": "Webapp",
  "description": "SQLMap is the gold standard...",
  "how_it_works": "SQLMap works by sending crafted HTTP requests...",
  "usage_scenarios": "Testing web applications for SQL injection...",
  "commands": ["sqlmap -u 'http://target/page?id=1' --dbs", ...],
  "strengths": ["Supports all 6 SQL injection techniques", ...],
  "weaknesses": ["Noisy - generates thousands of requests", ...],
  "comparison": "jSQL Injection offers a GUI alternative...",
  "detailed": true
}
```

## Author

**Cysec Don** - [GitHub](https://github.com/cysec-don)

## License

This project is provided for educational and security research purposes. All tools described are part of the BlackArch Linux open-source repository.

---

*BlackArch Linux: The Definitive Arsenal - Because knowing your tools is the first step to mastering them.*
