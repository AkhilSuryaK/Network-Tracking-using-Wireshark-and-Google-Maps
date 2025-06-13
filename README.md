🛰️ Network Traffic Visualization using Python, Wireshark, and Google Maps
This project captures network traffic using Wireshark, analyzes it with Python, maps the IP locations using the GeoLiteCity database, and visualizes the results on Google Maps through a .kml file.

📌 Features
Extracts IP addresses from captured .pcap files

Resolves IPs to geolocations using GeoLiteCity database

Outputs KML file to visualize connections on Google My Maps

Built with dpkt, socket, and pygeoip

🛠️ Technologies Used
Python 3.x

Wireshark

GeoLiteCity.dat (IP geolocation database)

Google My Maps for visualization

Python Libraries: dpkt, socket, pygeoip

📂 Project Structure
network-tracking-project/
├── wire.pcap → Network traffic capture file (not uploaded to GitHub)
├── GeoLiteCity.dat → IP geolocation database (not uploaded to GitHub)
├── main.py → Python script to process and generate KML
├── README.md → Project documentation
├── .gitignore → Ignore large/unused files

🚀 How to Run
1. Capture Traffic with Wireshark

Open Wireshark

Start capture on an active network interface

Stop and export traffic as wire.pcap

2. Download GeoLiteCity Database

Download from GitHub: https://github.com/mbcc2006/GeoLiteCity-data

Save as GeoLiteCity.dat in your project root folder

3. Install Required Libraries
Use pip to install the required libraries:
pip install dpkt pygeoip

4. Edit main.py
Update your public IP address inside the retKML() function like this:
src = gi.record_by_name('your.public.ip.address')
(Replace 'your.public.ip.address' with your actual IP, e.g., from https://www.whatsmyip.org/)

5. Run the Script
Run this command:
python main.py > output.kml
This will generate a .kml file containing all your network paths.

🗺️ Visualize on Google Maps
Go to https://www.google.com/mymaps

Click on "Create a new map"

Click Import on the first layer

Upload the generated output.kml file

Your network traffic will be visualized as lines connecting IP locations
