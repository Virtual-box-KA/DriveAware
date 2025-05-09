# DriveAware
## DriveAware v2 — Advanced Smart Road Safety & Vehicle Accident Prevention System

**DriveAware v2** represents a significant advancement in intelligent road safety infrastructure. Building upon the foundational features of the first prototype, this version introduces a more comprehensive and adaptive system that leverages **multi-modal sensing**, **deep learning**, **edge computing**, and **IoT connectivity** to deliver real-time hazard detection, alert generation, and remote monitoring capabilities.

Designed with challenging terrains like **mountain roads, blind curves, and poorly lit zones** in mind, DriveAware v2 also scales effectively to **urban intersections, school zones, and industrial traffic management systems**.

---

### 🔑 Key Components

- **Piezoelectric Sensor**: Detects mechanical vibrations, such as vehicle impacts, road knocks, or bumps — adding an extra layer of event detection beyond motion sensing.
- **ESP32-CAM Module**: Captures real-time video/images upon impact or vibration, runs AI-based image recognition using models trained on **Edge Impulse**, and manages data transmission.
- **Arduino Uno**: Interfaces with the piezo sensor and controls local alert mechanisms such as buzzers and LEDs, integrating seamlessly with the AI model for intelligent decision-making.
- **LEDs & Buzzer**: Provide instant visual and audio feedback to drivers in the event of detected hazards.
- **Wi-Fi Module (ESP8266/ESP32)**: Enables cloud integration, real-time data transmission, and remote access by authorities and administrators.

---

### ⚙️ System Architecture & Operational Flow

1. **Vibration Detection**  
   Piezoelectric sensors are installed at critical points to sense significant mechanical disturbances — indicative of vehicular motion, accidents, or unsafe driving conditions.

2. **Event-Triggered Imaging**  
   Upon vibration, the ESP32-CAM module captures images or streams live video. Data is either processed on-device or forwarded to edge systems (e.g., Jetson Nano, Raspberry Pi) for deep learning analysis.

3. **Object and Vehicle Recognition**  
   Leveraging **Edge Impulse** for model training, the system uses pre-trained AI models to perform real-time detection and classification of objects (e.g., vehicles, pedestrians), even under low-light or adverse weather conditions.

4. **Alert Generation**  
   Once a hazard is identified, the system activates LEDs and buzzers to notify nearby drivers. Optional display boards show object-specific warnings (e.g., “Vehicle Approaching”, “Pedestrian Detected”).

5. **IoT Integration & Remote Monitoring**  
   Critical data (images, event type, timestamp, location) is transmitted via Wi-Fi to cloud servers or mobile apps. Road authorities can monitor live feeds and access event logs in real time.

6. **Smart Communication Protocols**  
   Incorporates **Vehicle-to-Infrastructure (V2I)** and **Vehicle-to-Vehicle (V2V)** protocols, enhancing collective situational awareness among drivers, smart traffic systems, and emergency responders.

---

### 🚀 Major Enhancements Over DriveAware v1

- **Dual-Sensor Architecture**: Combines physical vibration detection with visual AI analysis for robust and redundant detection.
- **Advanced Object Differentiation**: Custom alerts based on object type (e.g., faster LED blinking for pedestrians, slower for cars).
- **Cloud Connectivity**: Facilitates long-term data storage, visualization, and predictive analytics.
- **Edge AI Acceleration**: Offloads computationally heavy tasks to edge devices to reduce latency and power usage.
- **Data Logging & Analytics**: All events are timestamped and stored for post-incident analysis and continuous model improvement.
- **Real-Time Decision Support**: Allows road authorities to assess threats and dispatch emergency or maintenance teams instantly.

---

### 🌐 Application Scope

While tailored for **mountainous regions** with sharp curves, poor lighting, and high risk of collisions, the modular design makes DriveAware v2 ideal for:
- Urban intersections and blind spots  
- School and hospital zones  
- Highway construction or detour sites  
- Industrial zones and loading docks  
- Parking lots and toll booths

---

### ✅ Benefits

- **Comprehensive Hazard Detection**: Combines mechanical and visual sensing with AI to reliably detect real-world dangers.
- **Real-Time, Proactive Safety**: Reduces accident response time and enables preventive actions.
- **Scalable and Affordable**: Designed using widely available components, ensuring cost-efficiency for deployment at scale.
- **Modular and Future-Proof**: Ready for integration with GPS, radar, GSM, RFID, and other evolving technologies.
- **Localized Decision-Making**: Reduces dependence on cloud infrastructure by enabling edge-based alerting and classification.

---

### 👥 Team Members

- **Keshav Agarwal**
- **Parkhi Sharma**
- **Kartikey Kumar**
- **Kirti Sharma**
> *DriveAware v2 aims to revolutionize smart road infrastructure through intelligent sensing, edge-based processing, and seamless IoT communication — offering a safer, smarter future for every road user.*

