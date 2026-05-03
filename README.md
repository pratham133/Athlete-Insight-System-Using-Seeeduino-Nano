🏃 Athlete Insight System (AIS)

📌 Overview  
The Athlete Insight System (AIS) is a low-cost, open-architecture wearable device developed for real-time monitoring of important fitness and health parameters such as step count, heart rate, blood oxygen saturation (SpO2), and calorie expenditure. Built around the Seeeduino Nano, the project combines embedded sensing, wireless communication, and mobile visualization into a compact and practical health-tracking platform.

✨ Key Features
>Real-time monitoring of heart rate, SpO2, step count, and calories

>Powered by the Seeeduino Nano (ATmega328P, 16 MHz)

>Uses BMA456 for motion sensing and MAX30102 for physiological monitoring

>Wireless Bluetooth communication through the HC-05 module

>Android dashboard built on Kodular for live data display and logging

>Optional SSD1306 OLED display for direct on-device feedback

>Complete hardware cost remains under USD 15

🧠 System Design  
AIS follows a four-layer architecture: sensing, processing, communication, and application. Sensor data is collected through the BMA456 and MAX30102, processed by the Seeeduino Nano, transmitted via Bluetooth, and displayed in real time on a custom Android application.

🛠️ Hardware Components
| Component          | Function                                                 |
| ------------------ | -------------------------------------------------------- |
| Seeeduino Nano     | Main controller and processing unit PUBLISHED-PAPER.pdf  |
| BMA456             | Step counting and activity detection PUBLISHED-PAPER.pdf |
| MAX30102           | Heart rate and SpO2 sensing PUBLISHED-PAPER.pdf          |
| HC-05              | Bluetooth communication PUBLISHED-PAPER.pdf              |
| SSD1306 OLED       | Local display output PUBLISHED-PAPER.pdf                 |
| 3.7V LiPo + TP4056 | Battery power and charge management PUBLISHED-PAPER.pdf  |

💻 Software Implementation  
>Firmware developed in Arduino IDE using C/C++

>Android application created using Kodular

>Data transmitted every 500 ms in ASCII CSV format

>SQLite logging used for storing monitored data

>Threshold alerts included for athlete safety monitoring

📊 Performance Metrics  
The prototype demonstrated reliable performance during experimental validation against reference devices. It achieved 95.8% step-count accuracy, 2.1 bpm resting heart-rate deviation, Bluetooth stability up to 10 meters with zero packet loss, latency below 200 ms, and average battery life of 6.2 hours.
| Metric               | Result                                   |
| -------------------- | ---------------------------------------- |
| Step Count Accuracy  | 95.8% (MAE 4.2%) PUBLISHED-PAPER.pdf     |
| Resting HR Deviation | 2.1 bpm ± 1.3 SD PUBLISHED-PAPER.pdf     |
| Motion HR Deviation  | 4.8 bpm ± 2.1 SD PUBLISHED-PAPER.pdf     |
| SpO2 Accuracy        | Within ±2% PUBLISHED-PAPER.pdf           |
| Bluetooth Range      | 10 m, 0% packet loss PUBLISHED-PAPER.pdf |
| App Latency          | < 200 ms PUBLISHED-PAPER.pdf             |
| Battery Life         | 6.2 hours average PUBLISHED-PAPER.pdf    |
| BOM Cost             | < USD 15 PUBLISHED-PAPER.pdf             |

🚀 Applications 
>Athlete fitness tracking

>Sports performance monitoring

>Wearable health-tech research

>Embedded and IoT project development

>Academic demonstration and prototyping

🔮 Future Scope   
Future enhancements include BLE integration for improved power efficiency, improved heart-rate accuracy, GPS support for outdoor tracking, and cloud or machine-learning integration for anomaly detection and athlete performance analysis.

🌍 Project Value  
AIS highlights how a meaningful wearable monitoring system can be built using affordable and reproducible hardware. Its open and research-friendly design makes it especially useful for students, academic projects, and developers exploring health-focused IoT solutions.
