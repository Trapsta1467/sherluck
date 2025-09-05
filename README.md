![Python](https://img.shields.io/badge/Python-3.6%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Offensive](https://img.shields.io/badge/Purpose-Offensive%20Redteam-red)

# 🔍 Sherluck - Advanced Personal Data Wordlist Generator

<img src="./SherluckLogo.png" alt="Sherluck Icon" width="300"/>

Sherluck is a powerful Python-based wordlist generator designed for cybersecurity professionals, penetration testers, and security researchers. It creates comprehensive password wordlists from personal data using advanced pattern recognition, leet speak transformations, and intelligent combinations.

## ✨ Features

- **🔤 Multi-format Support**: Handles both single values and arrays in JSON input
- **⚖️ Weighted Generation**: Prioritizes words based on importance weights
- **🎯 Leet Speak Generation**: Creates multiple leet speak variations for each word
- **🔗 Smart Combinations**: Generates 2-word and 3-word combinations with various separators
- **📅 Date Intelligence**: Extracts and utilizes date components from birthdates and anniversaries
- **🎭 Prefix/Suffix Integration**: Applies common prefixes and suffixes to enhance word variations
- **🌐 External Wordlists**: Optional integration with popular wordlists (rockyou, common passwords, etc.)
- **⚡ Multi-threading**: Parallel processing for faster generation
- **📏 Length Filtering**: Customizable minimum and maximum password lengths

## 🚀 Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/sherluck.git
cd sherluck

# Install dependencies
pip install requests

# Make the script executable
chmod +x sherluck.py
```

## Basic Usage
```bash
python sherluck.py -i person.json -o wordlist.txt
```

## Advanced Options
```bash
# With common wordlists and custom length
python sherluck.py -i person.json -o wordlist.txt --include-common --min-length 6 --max-length 25

# Disable multi-threading for older systems
python sherluck.py -i person.json -o wordlist.txt --no-threading

# Use specific common wordlists
python sherluck.py -i person.json -o wordlist.txt --include-common --common-lists rockyou common_passwords
```


## Default Weight Categories:

- basic: 1.0 (names, nicknames) 
- family: 0.9 (family members, pets) 
- relationships: 0.8 (friends, partners) 
- education: 0.7 (schools, universities) 
- work: 0.6 (companies, workplaces) 
- favorites: 0.8 (favorite things) 
- dates: 0.9 (birthdates, anniversaries)

## ⚠️ Legal Disclaimer

This tool is intended for:

- Security research and penetration testing
- Educational purposes
- authorized security assessments

Always ensure you have proper authorization before using this tool on any system. Never use it for unauthorized access or malicious activities.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.