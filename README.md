# Pcap Analysis 

## Overview
This Python script is designed to analyze pcap files for interactions involving a specific IP address. It filters packets to only those involving the target IP address, extracts information about each packet, and provides a summary of communication between IP addresses on each port.

## Requirements
- Python 3.x
- scapy library (install via `pip install scapy`)

## Usage
1. Clone or download the script `pcap_analyzer.py`.
2. Open a terminal or command prompt.
3. Navigate to the directory containing the script.
4. Run the script with the following command:
```
python pcap_analyzer.py -p <path_to_pcap_files> -i <target_ip_address>
```
- Replace `<path_to_pcap_files>` with the path to the pcap file(s) or folder containing pcap files. Use `*` to select all files in a folder.
- Replace `<target_ip_address>` with the IP address you want to analyze.

## Example
To analyze all pcap files in a folder named `pcap_files` for interactions involving the IP address `192.168.1.100`, run the following command:
```
python pcap_analyzer.py -p pcap_files/* -i 192.168.1.100
```

## Output
The script outputs information about each packet involving the target IP address and provides a summary of communication between IP addresses on each port.

## Notes
- Ensure that you have appropriate permissions to read the pcap files.
- The script utilizes the scapy library for packet manipulation and analysis.
