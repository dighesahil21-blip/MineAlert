# MineAlert
📌 Overview
MineAlert is an advanced Vehicle-to-Vehicle (V2V) and Vehicle-to-Infrastructure (V2I) anti-collision, real-time fleet telemetry, and zero-visibility voice dispatch platform designed for heavy-earth-moving machinery (HEMM) operating in rugged, high-fog, or zero-cellular-connectivity open-cast mines.

Operating independently of cellular network towers, the system uses decentralized LoRa 433MHz Mesh Networking, local 24GHz Radar (CDM324), NEO-6M GPS, and MPU-6050 IMU sensor telemetry to prevent collisions, stream real-time hazard warnings, and provide multi-lingual voice alerts to operators during thick monsoon fogs and blind switchback turns.

🚀 Key Features & Capabilities
🗺️ Bailadila Haul Road GIS & 3D Digital Twin:

Real-time Three.js WebGL simulation mapping switchback ridge crests, active haul loops, and dynamic fog density profiles.

Live 3D orbital camera tracking allowing dispatchers to instantly jump to any active dumper truck in the fleet.

📡 Decentralized LoRa 433MHz Mesh Telemetry:

Autonomous peer-to-peer packet hopping (SX1278 transceiver simulation) ensuring robust communication across steep mountain ridges with zero internet dependency.

Live packet inspector, RSSI/SNR signal quality charts, and raw hex payload telemetry stream.

⚠️ Proximity & Collision Avoidance HUD:

Multi-tier safety zones: Safe (>50m), Caution (30–50m), and Danger (<30m) with Time-To-Collision (TTC) tracking.

Integration with 24GHz radar obstacle detection and IMU pitch/roll sensors for grade monitoring and tire-slip/deceleration alerts.

🗣️ Multilingual Voice Dispatch:

Regional voice alerts and UI translations tailored for operators in multiple Indian languages and dialects (Hindi, Telugu, Kannada, Odia, Chhattisgarhi, Bengali, and English).

📊 Productivity & Safety Analytics Dashboard:

Tracks ore evacuated (tonnes), cycle times, monsoon production savings, and automated near-miss prevention statistics.

🛠️ Technology Stack
Frontend / UI: HTML5, Modern CSS3, JavaScript (ES6+), Tailwind/Custom Flexbox Styling

3D Visualization: Three.js (WebGL Digital Twin)

Data Visualization & Graphs: Chart.js / Canvas API

Embedded IoT Spec:

Microcontroller: ESP32 (240MHz Core)

RF Communication: SX1278 LoRa Module (433.175 MHz Mesh)

Positioning: NEO-6M GPS (NMEA 0183)

Proximity/Motion: 24GHz CDM324 Radar & MPU-6050 6-Axis IMU

MineAlert/
├── index.html          # Main dashboard & single-page application interface
├── css/
│   └── style.css       # Custom dark-mode mining HUD styling & responsive layouts
├── js/
│   ├── app.js          # Core application logic, telemetry loop & state management
│   ├── three-scene.js  # 3D Digital Twin Haul Road & Truck rendering
│   └── lora-mesh.js    # LoRa packet stream simulator & spectrum waterfall
└── assets/
    └── icons/          # Fleet, radar, and UI indicator graphics

    🏃‍♂️ Running Locally
To run or modify this project locally:

Clone the repository:

Bash
git clone https://github.com/dighesahil21/MineAlert.git
Navigate to the project directory:

Bash
cd MineAlert
Open index.html directly in your web browser, or serve it using a local development server (e.g., Live Server extension in VS Code).

🏆 Impact & Use Cases
Zero Fog Halt Days: Eliminates production downtime during heavy monsoon fogs by enabling blind-spot navigation and telemetry tracking.

Enhanced Operator Safety: Real-time visual and voice prompts prevent switchback collisions on steep mountain gradients.

Cost Efficiency: Proven reduction in near-miss incidents and increased annual ore evacuation output.


