## ESP32 RTOS OTA Update ![ESP32](https://img.shields.io/badge/ESP32-blue.svg) ![OTA](https://img.shields.io/badge/OTA-green.svg) ![FreeRTOS](https://img.shields.io/badge/FreeRTOS-orange.svg) ![Incomplete](https://img.shields.io/badge/Project_Incomplete-E50A00)

### Project Overview

The **ESP32 RTOS OTA Update** project implements an over-the-air (OTA) update mechanism using FreeRTOS on the ESP32 platform. The device enters OTA mode when a button is long pressed.

## Project Milestones

### Milestone 1: Project Initialization
- **Status:** Completed
- **Description:** Setup project repository and initial project structure.
  
### Milestone 2: FreeRTOS Integration
- **Status:** Completed
- **Description:** Integrate FreeRTOS with ESP32 and create basic tasks.

### Milestone 3: Button Input Handling
- **Status:** Completed
- **Description:** Implement button press and long press detection.

### Milestone 4: OTA Mode Implementation
- **Status:** Completed
- **Description:** Implement HTTPS OTA mode when the button is long pressed.

### Milestone 5: Testing and Debugging
- **Status:** Ongoing
- **Description:** Test the OTA functionality and debug any issues.

## Project Status ![Project Status](https://img.shields.io/badge/Status-Working-green.svg)

- The project is currently functional in OTA mode.

## How to Use

### Prerequisites
- **Hardware:** ESP32 Development Board
- **Software:** 
  - Visual Studio Code
  - ESP-IDF v5.00 or above

### Setup Instructions

1. **Clone the Repository:**
   ```sh
   git clone https://github.com/negedger/espidf-ota.git
   cd espidf-ota
   ```

2. **Set Up ESP-IDF:**
   Follow the [ESP-IDF setup guide](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html) to configure your development environment.

3. **Configure Project:**
   ```sh
   idf.py menuconfig
   ```
   - Set your Wi-Fi SSID and password under `Component config` -> `Wi-Fi`.

4. **Build and Flash the Project:**
   ```sh
   idf.py build
   idf.py -p (PORT) flash
   ```

5. **Monitor the Output:**
   ```sh
   idf.py -p (PORT) monitor
   ```

### OTA Update Process
- Long press the designated button on your ESP32 board.
- The ESP32 will enter OTA mode and start the update process if a new firmware is available.

 
### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

----
