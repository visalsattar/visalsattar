<div align="center">

# VISAL SATTAR
### NETWORK DEFENSE | COMPUTER VISION | APPLIED MACHINE LEARNING

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1000&color=00E5FF&center=true&vCenter=true&width=620&lines=%3E_SYSTEM_ONLINE_ID%3A_VISAL_SATTAR;%3E_INITIALIZING_AI_THREAT_DETECTION...;%3E_INSPECTING_FLOW_PACKETS_AT_LINE_RATE...;%3E_RUNNING_YOLOv8_COMPUTER_VISION_INFERENCE...;%3E_ALL_SYSTEMS_OPERATIONAL" alt="Terminal Typing SVG" />
</p>

[![Location](https://img.shields.io/badge/LOCATION-PESHAWAR_PK-0D1117?style=for-the-badge&logo=googlemaps&logoColor=00E5FF)](#)
[![Education](https://img.shields.io/badge/B.S._COMPUTER_SCIENCE-UAP-0D1117?style=for-the-badge&logo=databricks&logoColor=00E5FF)](#)
[![Security+](https://img.shields.io/badge/SECURITY%2B-TARGET_DEC_2026-0D1117?style=for-the-badge&logo=comptia&logoColor=00E5FF)](#)
[![Email](https://img.shields.io/badge/SECURE_COMMS-VISAL2105@AUP.EDU.PK-0D1117?style=for-the-badge&logo=minutemailer&logoColor=00E5FF)](mailto:visal2105@aup.edu.pk)

</div>
<br>

### 🖧 CORE FOCUS & CAPABILITIES

Computer Science undergraduate (Expected May 2026) specializing in network defense pipelines and computer vision automation. Focused on capturing raw traffic, training ensemble threat classifiers, and deploying containerized, real-time ML applications.

- 🛡️ **Network Security:** Real-Time Flow Analysis, Packet Sniffing, Threat Intelligence Lookups, NIST SP 800-30 Alignment
- 👁️ **Computer Vision:** YOLOv8 Object Detection, Image Segmentation, Dataset Preprocessing & Fine-Tuning
- ⚙️ **Systems & Infrastructure:** Docker Containerization, Redis Streams, Flask APIs, Linux/PowerShell Scripting
- 🎯 **Target Roles:** SOC Analyst | Junior Cybersecurity Analyst | ML/Security Software Engineer

---

### 🛡️ FEATURED PROJECT 01: AI-BASED INTRUSION DETECTION SYSTEM (IDS)

> Real-time ensemble network anomaly detection pipeline benchmarked against the CICIDS2017 dataset. A CNN architecture was separately trained and evaluated offline for comparison purposes only — it is not part of the live fusion pipeline.

```mermaid
graph LR
    A((Live Network Traffic)) --> B[Scapy & cicflowmeter: <br> Packet Ingestion]
    B --> C{ML Fusion Layer}
    C --> D[Random Forest: <br> 99.50% F1]
    C --> E[Autoencoder: <br> Anomaly Detection]
    D --> F[(Redis Streams: <br> Message Queue)]
    E --> F
    F --> G[React Dashboard <br> via WebSockets]

    classDef default fill:#0D1117,stroke:#00E5FF,stroke-width:1px,color:#E6EDF3;
    classDef highlight fill:#00E5FF,stroke:#00E5FF,color:#000000;
    class A,G highlight;
```

- **Engineered Real-Time Ingestion:** Processed live network flow data with Scapy and cicflowmeter inside isolated Python virtual environments.
- **Ensemble Threat Classification:** Benchmarked classification models against the CICIDS2017 dataset (225,745 flows), achieving a 99.50% F1-score on the live Random Forest classifier (a CNN variant was evaluated offline at 99.51% F1 for architecture comparison — not deployed in the live pipeline).
- **Live Intelligence Enrichment:** Streamed alerts via WebSockets and Redis Streams to a React dashboard with integrated GeoIP and AbuseIPDB threat intelligence.
- **Container Deployment:** Containerized full-stack services using Docker; the packet-capture service requires elevated `NET_ADMIN`/`NET_RAW` capabilities to read raw traffic (documented and scoped to that container only).

**Tech Stack:** Python 3.11 | cicflowmeter | Scapy | TensorFlow | scikit-learn | Redis | Docker | React

---

### 🎯 FEATURED PROJECT 02: YOLOv8 WASTE DETECTION & SEGMENTATION ENGINE

Computer vision pipeline fine-tuned on ICRA Trash & Drinking Waste datasets for automated visual identification.

```mermaid
graph LR
    A((Raw Image Input)) --> B[OpenCV / Python: <br> Data Preprocessing]
    B --> C{YOLOv8 PyTorch Engine}
    C --> D[Object Bounding Box Detection]
    C --> E[Instance Image Segmentation]
    D --> F[Flask Web Application API]
    E --> F
    F --> G[Structured Inference <br> & Visual Output]

    classDef default fill:#0D1117,stroke:#00E5FF,stroke-width:1px,color:#E6EDF3;
    classDef highlight fill:#00E5FF,stroke:#00E5FF,color:#000000;
    class A,G highlight;
```

- **Custom Model Fine-Tuning:** Trained YOLOv8 object detection and segmentation architectures across diverse environmental waste categories.
- **Inference Web Service:** Integrated trained models into a lightweight Flask web application to process image uploads and stream structured bounding-box detections.
- **Data Preprocessing Pipeline:** Automated data cleaning, bounding box normalization, and validation augmentation across multi-source benchmark datasets.

**Tech Stack:** Python | YOLOv8 | Flask | OpenCV | Jupyter Notebook | PyTorch

---

### 💼 PROFESSIONAL EXPERIENCE

**Web Development & Database Intern | Ministry of Agriculture — Bureau of Agriculture Information Dept.**
*Jun 2024 – Dec 2024*
- Streamlined department reporting workflows by architecting 12+ optimized relational SQL database queries, reducing weekly manual report generation time by ~80%.
- Deployed an internal JavaScript operational time-tracking utility adopted by 25+ departmental staff members, replacing legacy manual logging processes.
- Developed responsive web application components using HTML5, CSS3, JavaScript, and Bootstrap, improving cross-device interface accessibility across department endpoints.

---

### 📜 CERTIFICATIONS & COURSEWORK

- **Google Cybersecurity Professional Certificate** — Google (Coursera)
- **CS50: Introduction to Computer Science** — HarvardX / edX
- **CompTIA Security+** — Target: Dec 2026 (not yet completed)
