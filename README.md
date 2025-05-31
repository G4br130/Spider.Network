# 🕸️ Spider.Network

**Spider.Network** is a sophisticated Python-based application that performs advanced network scanning and visualizes your entire network topology in an interactive **3D web interface** using **Three.js** embedded in **Streamlit**. It combines local network analysis, traceroute visualization, GeoIP geolocation, port inspection, and dynamic data representation to give a complete understanding of your digital environment.

---

## 🚀 Features

- 🔍 **Comprehensive Network Scan**
  - Detects all active devices on the local network (LAN)
  - Displays:
    - IP address
    - Hostname
    - MAC address and vendor
    - Open ports
    - Device role (gateway, client, unknown)

- 🛰️ **Traceroute Visualization with GeoIP**
  - Performs traceroute (`tracert` or `traceroute`) to a specified public IP (e.g., Google DNS)
  - Identifies all hops and their geographical locations
  - Maintains connection paths and visual link chains in 3D
  - Retrieves ASN (Autonomous System Number) and region info

- 🌐 **Local Device Details**
  - Displays your local IP address
  - Hostname
  - Default gateway
  - Public IP and ASN (via external API)

- 🕸️ **3D Topology Map (Three.js + Streamlit)**
  - Animated graph of network nodes and paths
  - Real-time packet animation along connection lines
  - Interactively rotate, zoom and inspect nodes
  - Color-coded devices (e.g., routers, servers, clients)

- 🧠 **Smart Filtering**
  - Filter by:
    - Device type
    - Port number
    - Location
    - Latency or number of hops

- 📊 **Final Data Summary**
  - Pandas DataFrame with:
    - All discovered IPs and metadata
    - Traceroute hops and GeoIP info
    - Exportable as `.csv` or `.json`

---

## 🧰 Technologies Used

| Tech        | Description                          |
|-------------|--------------------------------------|
| Python 3.10+| Core programming language             |
| Streamlit   | Web app UI and dashboard              |
| Three.js    | 3D rendering engine (via WebGL)       |
| Scapy       | Network packet manipulation           |
| Socket & Subprocess | System-level diagnostics     |
| GeoIP2      | Geolocation based on IP               |
| Pandas      | Data analysis and export              |
| Plotly / PyDeck (optional) | Interactive data viz  |

---

## 📦 Installation

```bash
git clone https://github.com/G4br130/Spider.Network/spider.network.git
cd spider.network
pip install -r requirements.txt
