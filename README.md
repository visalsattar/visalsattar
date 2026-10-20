<div align="center">

# VISAL SATTAR
### NETWORK DEFENSE | COMPUTER VISION | APPLIED MACHINE LEARNING

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1000&color=00E5FF&center=true&vCenter=true&width=700&lines=%3E_BS_COMPUTER_SCIENCE_2026;%3E_BUILT_AN_AI-ASSISTED_INTRUSION_DETECTION_SYSTEM;%3E_CAPTURING_LIVE_PACKETS_WITH_SCAPY...;%3E_FINE-TUNING_YOLOv8_FOR_WASTE_DETECTION...;%3E_SEEKING_ENTRY-LEVEL_SOC_ROLES" alt="Terminal Typing SVG" />
</p>

[![Location](https://img.shields.io/badge/LOCATION-PESHAWAR_PK-0D1117?style=for-the-badge&logo=googlemaps&logoColor=00E5FF)](#)
[![Education](https://img.shields.io/badge/B.S._COMPUTER_SCIENCE-MAY_2026-0D1117?style=for-the-badge&logo=databricks&logoColor=00E5FF)](#)
[![Security+](https://img.shields.io/badge/SECURITY%2B-IN_PROGRESS_DEC_2026-0D1117?style=for-the-badge&logo=comptia&logoColor=00E5FF)](#)
[![Email](https://img.shields.io/badge/EMAIL-VISALSATTAR.DEV-0D1117?style=for-the-badge&logo=minutemailer&logoColor=00E5FF)](mailto:visalsattar.dev@gmail.com)

[LinkedIn](https://linkedin.com/in/visalsattar) · [GitHub](https://github.com/visalsattar)

</div>
<br>

### 🖧 CORE FOCUS & CAPABILITIES

Computer Science graduate (BS, May 2026, The University of Agriculture, Peshawar). I build network security tools and machine-learning applications: capturing live traffic, scoring it with trained models, and showing the results in a real-time dashboard. I'm looking for an entry-level SOC or cybersecurity analyst role.

- 🛡️ **Network Security:** Live packet capture, intrusion detection, network traffic analysis, GeoIP and AbuseIPDB lookups
- 🔧 **Hands-on Tools:** Wireshark, Nmap, Scapy, Npcap, Linux, Windows, Docker
- 👁️ **Computer Vision:** YOLOv8 object detection and segmentation, dataset preparation, fine-tuning
- ⚙️ **Systems & Infrastructure:** Docker Compose, Redis Streams, Flask, Socket.IO
- 🎯 **Looking For:** SOC Analyst | Junior Cybersecurity Analyst | Security or ML Software Engineer

---

### 🛡️ FEATURED PROJECT 01: AI-BASED INTRUSION DETECTION SYSTEM (IDS)
**[Repository →](https://github.com/visalsattar/AI-Based-Intrusion-Detection-System-for-Real-Time-Threat-Detection)** · Final-year project, Nov 2025 – May 2026

> My final year project (Nov 2025 – May 2026): a real-time pipeline that captures network traffic, scores it with a Random Forest and an Autoencoder trained on CICIDS2017, and sends enriched alerts to a React dashboard. A CNN was trained offline for comparison and is not part of the live pipeline.

```mermaid
graph LR
    A((Live Network Traffic)) --> B[Scapy + Npcap: <br> Packet Capture]
    B --> C[Flow Feature <br> Extraction]
    C --> D{Fusion Layer}
    D --> E[Random Forest]
    D --> F[Autoencoder]
    E --> G[(Redis Streams)]
    F --> G
    G --> H[React Dashboard <br> + GeoIP / AbuseIPDB]

    classDef default fill:#0D1117,stroke:#00E5FF,stroke-width:1px,color:#E6EDF3;
    classDef highlight fill:#00E5FF,stroke:#00E5FF,color:#000000;
    class A,H highlight;
```

- **Live Capture:** A Scapy sniffer runs on the Windows host through Npcap (as Administrator) and captures TCP and UDP traffic. My own feature extractor rebuilds the 78 CICFlowMeter flow features the models were trained on from packet headers and timing.
- **Results:** Evaluated on a chronological held-out split (45,149 flows) of the CICIDS2017 DDoS file (225,745 rows). The Random Forest reached 99.50% F1. The Autoencoder reached 53.78% F1 (59.78% precision, 48.88% recall) at its operating point. Both numbers are as measured, and they cover DDoS traffic only.
- **Real-Time Alerts:** Detections flow through Redis Streams to Flask and out to the React dashboard over Socket.IO, enriched with GeoIP and AbuseIPDB data. Unconfirmed anomaly alerts are capped at MEDIUM severity so they can't trigger blocking.
- **Deployment:** Redis, Flask, and React run in Docker Compose; capture stays on the host. The backend waits for Redis to pass its healthcheck before it starts, so a slow Redis start doesn't crash it.
- **Testing:** I checked data cleaning, alert severity thresholds, and service startup by hand, and confirmed a constructed test alert reaches the dashboard end to end.
- **Not Done Yet:** No end-to-end capture-to-browser latency measurement (only Redis-to-dashboard delivery, 2.5 ms median, is measured), a pytest suite that is only scaffolded, and no attack testing on real network hardware.

**Tech Stack:** Python 3.11 | Scapy | Npcap | TensorFlow/Keras | scikit-learn | Flask | Redis Streams | Socket.IO | React | Docker Compose

**Link:** https://github.com/visalsattar/AI-Based-Intrusion-Detection-System-for-Real-Time-Network-Threat-Detection

---

### 🎯 FEATURED PROJECT 02: YOLOv8 WASTE DETECTION & SEGMENTATION ENGINE
**[Repository →](https://github.com/visalsattar/yolo_detection_app)** · Personal project, Feb 2024 – Dec 2024

A Flask web app (Feb 2024 – Dec 2024) that takes an uploaded image and returns detected and segmented waste items, using YOLOv8 models fine-tuned on the ICRA Trash and Drinking Waste datasets.

```mermaid
graph LR
    A((Uploaded Image)) --> B[OpenCV / Python: <br> Data Preparation]
    B --> C{YOLOv8 PyTorch Models}
    C --> D[Object Bounding Box Detection]
    C --> E[Instance Segmentation]
    D --> F[Flask Web Application]
    E --> F
    F --> G[Structured Results <br> & Visual Output]

    classDef default fill:#0D1117,stroke:#00E5FF,stroke-width:1px,color:#E6EDF3;
    classDef highlight fill:#00E5FF,stroke:#00E5FF,color:#000000;
    class A,G highlight;
```

- **Model Fine-Tuning:** Fine-tuned YOLOv8 detection and segmentation models on waste categories from the ICRA datasets.
- **Web Service:** A Flask app that accepts image uploads and returns structured bounding-box results.
- **Data Preparation:** Cleaned the data, normalized bounding boxes, and applied validation augmentation with OpenCV and Python.

**Tech Stack:** Python | YOLOv8 | PyTorch | OpenCV | Flask | Jupyter Notebook

**Link:** https://github.com/visalsattar/yolo_detection_app

---

### 💼 PROFESSIONAL EXPERIENCE

**Web Development & Database Intern | Ministry of Agriculture — Bureau of Agriculture Information Dept.**
*Jun 2023 – Dec 2023*
- Built responsive intranet web pages with HTML5, CSS3, JavaScript, and Bootstrap so staff could use them on phones, tablets, and desktops.
- Designed relational SQL schemas and wrote the queries used for internal data extraction and reporting.
- Wrote a JavaScript time-tracking tool for internal use.

---

### 📜 CERTIFICATIONS & TRAINING

- **Google Cybersecurity Professional Certificate** — Google (Coursera), completed May 2026
- **CompTIA Security+** — in progress, exam planned for Dec 2026
