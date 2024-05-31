## Autonomous Military Rover

This project details the design and development of a high-performance autonomous rover for military applications.

### Features

* Rugged iron chassis for durability in harsh environments.
* Tracks for increased traction on challenging terrains.
* 360-degree night vision camera for low-light visibility.
* Audio feed capabilities for situational awareness.
* GNSS location broadcasting and integrated navigation system for precise positioning.
* Autonomous path planning and obstacle avoidance using computer vision and deep learning.
* Real-time camera feed and location coordinates accessible via wireless control for remote monitoring.
* Modular design with mountable sections for customization (fire fighting, mine detection, robotic arm, etc.).

### Components

**Structure:**

* Rugged iron chassis
* Wheels
* Belts
* Batteries

**Motion:**

* Chain
* Suspension

**Electronics:**

* 2-channel ESC (motor speed controller)
* NVIDIA Jetson Nano (SBC - AI computing platform)
* Pixhawk (Ardupilot - autopilot flight controller)
* 12V DC gear motors (x4)
* 18V 6Ah battery (power supply)
* DC-DC regulator (5V 10A - voltage converter)
* 75mm GPS pole (GPS antenna mount)
* Microphone module (sound input device)
* LoRa module (long-range communication)
* RF module (radio frequency communication)
* RF controller remote (remote control unit)
* Camera module (image capturing device)
* Microcontroller (control unit)
* MPU-6050 (motion sensing - accelerometer and gyroscope)
* LiDAR sensor (light detection and ranging)
* Obstacle avoidance sensor
* LEDs (light indicators)
* Buzzers (audio alerts)

**Other Accessories:**

* Mounts
* Screws and nuts
* Cooling fan
* Data storage (SSD/SD card)
* Wiring and connectors
* Gearbox

### Software (Mission Planner)

Mission Planner is a ground control station software used for configuration and dynamic control of the rover's autonomous navigation and obstacle detection.

### Live Camera/Video Streaming and Storage

* Live camera feed for real-time situational awareness and mission control.
* Web-based interface for remote access to the live camera stream.
* Video recording stored on SD card for later retrieval.

### Mechanism of Motion

* Pixhawk autopilot module controls motors, sensors, and navigation algorithms.

### Hardware Components

* **2-channel ESCs:** Control speed and direction of the motors based on commands from Pixhawk.
* **12V DC Gear Motors:** Provide driving force.
* **NVIDIA Jetson Nano:** Central processing unit that runs autopilot software, obstacle detection algorithms, and sensor fusion software.
* **Pixhawk (Ardu-pilot):** Autopilot flight controller that translates commands from Jetson Nano into signals for the ESCs.
* **Camera Module:** Captures images and video for obstacle detection, navigation, and situational awareness.
* **LiDAR Sensor:** Creates a 3D point cloud of the surroundings for obstacle detection and path planning.

### Additional Sensors

* **MPU-6050:** Provides data on the rover's orientation for stability.
* **Obstacle Avoider Sensor:** Ultrasonic or infrared sensor for short-range obstacle detection.

### Motion Control and Sensor Fusion

* Pixhawk receives control commands from Jetson Nano (user input or autonomous navigation algorithms).
* Jetson Nano uses camera image data and LiDAR point cloud for obstacle detection and environment perception.
* Sensor fusion combines camera image and LiDAR data for a richer environment representation.
* Obstacle detection algorithms identify potential obstacles.
* Jetson Nano sends control commands to Pixhawk based on processed sensor data and obstacle detection.
* Pixhawk translates commands into signals for ESCs, controlling motor speed and direction for autonomous navigation and obstacle avoidance.

### Societal Applications

* Search and rescue in hazardous areas (fires, collapsed buildings) by locating survivors and transmitting real-time data.
* Disaster response and civilian applications.

### Prototype Sizes

* Proof of concept (small version): 30 cm x 20 cm x 20 cm
* Actual version (prototype): 45 cm x 30 cm x 20 cm

### Development Timeline

* Phase 1: Design and Development (45 days) - Design, component selection, and initial software development.
* Phase 2: Prototyping and Testing (90 days) - Building and testing the rover prototype.
* Phase 3: Refinement and Validation (90 days) - Refining the design and software based on testing, final testing, and deployment preparation.
* Total estimated timeline: 225 days
░
