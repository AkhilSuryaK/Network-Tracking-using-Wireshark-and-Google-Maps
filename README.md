# Network-Tracking-using-Wireshark-and-Google-Maps
# Network Traffic Visualization using Python, Wireshark, and Google Maps

This project captures network traffic using Wireshark, converts it into geographic coordinates using GeoLiteCity, and visualizes it on Google Maps via KML.

## How to Use
1. Capture network traffic using Wireshark and save as `wire.pcap`.
2. Run the Python script: `python main.py`
3. Copy the output and save it as a `.kml` file.
4. Upload the KML file to [Google My Maps](https://www.google.com/mymaps).

## Requirements
- Python 3.x
- Libraries: `dpkt`, `socket`, `pygeoip`
