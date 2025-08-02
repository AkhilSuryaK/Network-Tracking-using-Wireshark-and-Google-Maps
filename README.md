# 🛰️ Network Traffic Visualization using Python, Wireshark, and Google Maps

A powerful network analysis project that captures live traffic, extracts IPs, maps geolocations using the **GeoLiteCity** database, and visualizes connections on **Google Maps** through a `.kml` file.

> 🔗 Live Demo: _Coming Soon_  
> 👨‍💻 Developed by [Kolipaka Akhil Surya](https://www.linkedin.com/in/akhilsurya/)

---

## 📌 Features

- 🌐 Extracts IP addresses from `.pcap` files captured by Wireshark
- 🌍 Resolves IPs to geographical locations using **GeoLiteCity**
- 🗺️ Generates a `.kml` file for Google My Maps visualization
- ⚙️ Built with **dpkt**, **socket**, and **pygeoip** libraries

---

## 🛠️ Technologies Used

- **Programming Language:** Python 3.x  
- **Traffic Capture Tool:** Wireshark  
- **Geo Database:** GeoLiteCity.dat  
- **Visualization:** Google My Maps  
- **Python Libraries:** `dpkt`, `socket`, `pygeoip`

---

## 📁 Project Structure



network-tracking-project/

├── wire.pcap # Captured traffic file

├── GeoLiteCity.dat # IP geolocation database

├── main.py # Python script to extract & generate .kml

├── output.kml # Output file for Google Maps (after running)

├── .gitignore # File to ignore large/unused files

└── README.md # Project documentation


---

## 🚀 How to Run

### 1️⃣ Capture Traffic with Wireshark

- Launch **Wireshark**
- Start capture on your active network interface
- Stop capture after some time
- Export the traffic as `wire.pcap` file

---

### 2️⃣ Download GeoLiteCity Database

- Download from this GitHub mirror:  
  [GeoLiteCity.dat](https://github.com/mbcc2006/GeoLiteCity-data)
- Save the `.dat` file as `GeoLiteCity.dat` in your project root

---

### 3️⃣ Install Required Python Libraries

```bash
pip install dpkt pygeoip

4️⃣ Edit main.py
Update your public IP address inside the retKML() function:
src = gi.record_by_name('your.public.ip.address')

🔄 Replace 'your.public.ip.address' with your actual IP
🌐 You can find it here: https://www.whatsmyip.org/

5️⃣ Run the Script
python main.py > output.kml

✅ This will generate a output.kml file with IP connection paths🗺️ Visualize on Google Maps
Go to Google My Maps
Click on "Create a new map"
Click Import on the first layer
Upload the output.kml file
Your network traffic will be shown as lines connecting IP locations

🧠 Use Case
This tool is useful for:
Network security analysis
Visualizing inbound/outbound traffic
Educational & cybersecurity demonstrations

📬 Contact
GitHub: @AkhilSuryaK
LinkedIn: Akhil Surya Kolipaka

📃 License
This project is licensed under the MIT License.

---

Let me know the next project you'd like a `README.md` for—I'll maintain the same quality and consistency!
  


