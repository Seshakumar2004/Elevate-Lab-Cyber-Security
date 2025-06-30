## 📡 Live Network Packet Capture using Wireshark

### 🎯 Objective
Capture live network packets and identify basic protocols and traffic types using Wireshark.

---

### 🛠️ Tools Used
- **Wireshark** – A free and open-source packet analyzer

---

### 🧪 Steps Performed

```bash
1. Installed and launched Wireshark.
2. Selected the active network interface for packet capture (Wi-Fi).
3. Started the live packet capture.
4. Visited websites and pinged servers to generate traffic.
5. Stopped the capture after ~1 minute.
6. Filtered captured packets using protocols like TCP, TLS, and ARP.
7. Exported the capture as a .txt file for analysis.
```

---

### 📄 Protocols Identified

| Protocol       | Description                            | Observed Use                              |
|----------------|----------------------------------------|-------------------------------------------|
| **TCP**        | Transmission Control Protocol           | Reliable data delivery (port 443)         |
| **TLSv1.2/1.3**| Transport Layer Security                | Encrypted HTTPS communication             |
| **ARP**        | Address Resolution Protocol             | IP-to-MAC address resolution in LAN       |

---

### 🌐 Notable External Services Accessed

Based on TLS packet SNI (Server Name Indication):

- `storage.live.com`  
- `onedriveclucprodbn20028.blob.core.windows.net`  
- `gateway.grammarly.com`  
- `extension.femetrics.grammarly.io`

---

### 📁 Deliverables

- ✅ Captured packet file: `network_capture.txt`
- ✅ Protocol analysis report: `protocol_summary.txt`

---

### 📌 Observations

- TLS traffic shows secure communication with cloud services.
- Multiple TCP handshakes observed for new connections.
- ARP exchanges confirm normal local network behavior.
