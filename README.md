
# IOC Extractor

A powerful CLI tool for extracting Indicators of Compromise (IOCs) from various file formats. Designed for cybersecurity professionals and digital forensics as my training project

## Features

- Extract IOCs from multiple file formats: PDF, DOCX, HTML, JSON, CSV, LOG and text files
-  Support for various IOC types: IP addresses, hashes, domains, URLs, emails, CVEs
- Multiple output formats: text, JSON, CSV
- Streaming mode for large files
- Validation of extracted IOCs
- Python-based with easy installation via pip

## Standard Installation

Install my-project with pip:

```bash
pip install ioc-extractor
```
### For Kali Linux Users 
Using pipx: 
```bash
sudo apt install pipx
pipx ensurepath
pipx install ioc-extractor
```  
## Usage/Examples
Getting Help
```bash
# Show main help with all available commands
ioc-extractor --help

# Show help for the extract command
ioc-extractor extract --help

# Show help for other commands
ioc-extractor formats --help
ioc-extractor types --help
```
<img width="1456" height="348" alt="image" src="https://github.com/user-attachments/assets/dedc8155-7004-4ac4-a829-c81d7f70acd0" />

Basic Extraction
```bash
ioc-extractor extract document.pdf
```
Save Results to a File
```bash
ioc-extractor extract document.pdf -o results.json -f json
```
Extract Specific IOC Types Only
```bash
ioc-extractor extract document.pdf --ipv4
```
<img width="963" height="279" alt="image" src="https://github.com/user-attachments/assets/b7bf2c2f-8d0c-4183-95ad-b31786e2eb84" />

View Supported Formats and IOC Types
```bash
ioc-extractor formats
ioc-extractor types
```
<img width="508" height="219" alt="image" src="https://github.com/user-attachments/assets/6674fb70-d1a9-4cd7-838f-f38117377513" />

## Building from Source
```bash
git clone https://github.com/deteyl/ioc-extractor.git
cd ioc-extractor
pip install -e .
```
