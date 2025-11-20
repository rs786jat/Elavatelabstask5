
# 📡 Network Packet Capture with Wireshark

## 🎯 Objective
Capture live network packets using **Wireshark** and identify basic protocols and traffic types.

## 🛠️ Tools
- **Wireshark** (Free, Open Source)

## 📂 Deliverables
- A packet capture file: `capture.pcap`
- A short report summarizing identified protocols and traffic types

---

## 📝 Steps Taken
1. Installed Wireshark on the system.  
2. Started capturing packets on the active network interface.  
3. Generated traffic by browsing a website and pinging a server.  
4. Stopped the capture after ~1 minute.  
5. Applied filters to view specific protocols (e.g., `http`, `dns`, `tcp`).  
6. Identified at least **3 different protocols** in the capture.  
7. Exported the capture as `capture.pcap`.  
8. Summarized findings in this README.

---

## 🔍 Protocols Identified
| Protocol | Purpose | Example Observations |
|----------|----------|----------------------|
| **DNS** | Resolves domain names to IP addresses | Queries to `google.com` and responses from DNS servers |
| **HTTP** | Web traffic between client and server | GET requests to websites, HTML responses |
| **TCP** | Reliable transport layer protocol | Handshakes (`SYN`, `ACK`) and data transfer segments |

---

## 📊 Findings
- **DNS traffic** shows name resolution requests whenever a website is accessed.  
- **HTTP packets** reveal browsing activity, including requests and responses.  
- **TCP segments** demonstrate connection setup and teardown, ensuring reliable communication.  
- The capture highlights how multiple protocols work together: DNS resolves names, TCP establishes connections, and HTTP delivers content.  

---

## 📁 Repository Structure
```
├── capture.pcap        # Packet capture file
├── README.md           # Documentation (this file)
```

---

## 🚀 How to Use
1. Open `capture.pcap` in Wireshark.  
2. Apply filters like:
   - `dns` → View DNS queries/responses  
   - `http` → Inspect web traffic  
   - `tcp` → Analyze transport layer packets  
3. Explore packet details to understand protocol behavior.  
