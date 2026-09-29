# 📶 Wireless Industrial Environmental Monitor & IoT Gateway

Exploring embedded systems, wireless communications, and factory data routing using the 32-bit ESP32 chip.

## 💡 The Motivation
Cables can be a major failure point in busy factory settings. Modern automation relies heavily on wireless IoT (Internet of Things) devices. I built this project to step up from foundational microcontrollers to higher-frequency 32-bit hardware with integrated radio units, learning how modern smart factories transfer machine data through the air without physical tethering.

## 🛠️ How the System Works
1. **The Wireless Node (Wokwi):** An ESP32 microcontroller initialises its internal Wi-Fi stack to simulate connecting to a local factory network. It reads environmental data from a DHT22 sensor and broadcasts the telemetry packets wirelessly over the local IP grid.
2. **The Diagnostic Hub (Google Colab):** A cloud-based Python script acts as a remote maintenance dashboard. It intercepts the incoming network strings, cleans the text to extract the raw measurements, and visualises the network performance.

## 🔗 Live Interactive Links
* **Live Virtual ESP32 Hardware Simulator:** [Launch the Wokwi Simulation](https://wokwi.com/projects/475945837938861057)
* **Cloud Network Parsing Dashboard:** [Open the Google Colab Notebook](https://colab.research.google.com/drive/1FcK2OKp9n9S4FbvYQw-NIEY_kfFjf1GQ?usp=sharing)

## 🧠 What I Learned & Practised
* **Wireless Systems Integration:** Interfacing with basic Wi-Fi network libraries and managing device IP data routing within microcontroller firmware.
* **Network String Parsing:** Writing Python logic to isolate individual numbers from continuous data text streams so the computer can process them.
* **Network Reliability Handling:** Programming code that handles network timeouts and attempts to safely reconnect if a wireless transmission drops.
* **Advanced Microcontrollers:** Moving from entry-level hardware to working with more powerful 32-bit chips used in modern industrial automation.

---

### 🚀 Future Steps
I intend to implement a basic web server directly onto the ESP32 chip, allowing me to view active factory-floor data directly on any web browser connected to the same local network.
