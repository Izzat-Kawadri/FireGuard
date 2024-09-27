# FireGuard 

**Project Name:** FireGuard  
**Graduation Project for:** Faculty of Computer and Automation  
**Inspiration:** The increasing number of forest fires in recent years, especially in Syria, motivated us to develop a project that can detect fires early to minimize their damage.

**Summary:** Design and Build Forest Fire Detection System Using WSN (Wireless Sensor Network)
## Table of Contents
1. [Introduction](#introduction)
2. [The Problem](#the-problem)
3. [Result of the Problem](#result-of-the-problem)
4. [Our Solution](#our-solution)
5. [System Description](#system-description)
6. [System Components](#system-components)
7. [Block Diagram (DFD)](#block-diagram)
8. [Technology & Hardware Used](#technology--hardware-used)
9. [Results and Conclusion](#results-and-conclusion)
10. [Future Efforts](#future-efforts)
11. [References](#references)
12. [Credits](#credits)

---

## 1. Introduction <a name="introduction"></a>
Forest fires have been increasingly devastating over the last few years, destroying thousands of hectares of forest land. In particular, our homeland Syria has faced significant damage from these fires. Early detection and prompt action are essential to minimize the destruction and protect both human lives and natural resources.

---

## 2. The Problem <a name="the-problem"></a>
The rapid spread of forest fires, combined with delayed detection, often results in large-scale damage. Traditional methods for detecting and reporting fires are slow and inefficient, which leads to delays in mobilizing firefighters and other emergency services. There is an urgent need for a solution that detects forest fires in real time and alerts the relevant authorities immediately, allowing them to respond faster.

---

## 3. Result of the Problem <a name="result-of-the-problem"></a>
Over the past years, there has been a sharp increase in the number of fires globally and specifically in Syria. Here are some real data:

- **Year 2020**: Over **500** fires were reported in forests across Syria, with **80,000 hectares** burned.
- **Year 2021**: Fires increased by **25%**, further damaging vast areas.
- **Year 2022**: **10% more** fires, causing irreversible environmental harm.

These numbers highlight the pressing need for a better detection and response system.

---

## 4. Our Solution <a name="our-solution"></a>
Our solution, **Fireguard**, is an IoT-based Wireless Sensor Network (WSN) system designed to detect forest fires early. The system consists of the following main components:

1. **Sensor Nodes**: Placed in strategic locations in forests to measure temperature, smoke, and gas levels.
2. **Gateway**: Collects data from sensor nodes and sends it to the backend server.
3. **Backend Server**: Stores data and processes it for real-time updates.
4. **Dashboard**: Allows fire centers to monitor forest conditions and take decisions.
5. **Mobile App**: Designed for firefighters to receive tasks and respond quickly.
6. **Landing Page**: A simple web interface to showcase Fireguard's features and updates.

---

## 5. System Description <a name="system-description"></a>
The **Fireguard** system is designed for efficient and low-power operation. Here's how it works:

1. **Sensor Nodes**: These nodes are equipped with various sensors (DHT11 for temperature, MQ9 for smoke and gases). They monitor environmental conditions in the forest. The nodes are connected to a gateway using LoRa communication, enabling long-range data transmission. The nodes are programmed to go into sleep mode to conserve power when not actively transmitting.
  
2. **Gateway**: The gateway gathers data from all sensor nodes and sends it to the backend server using Wi-Fi or a cellular connection.

3. **Backend Server**: The server processes the data, stores it in a MySQL database, and updates the fire center's dashboard.

4. **Dashboard**: The dashboard provides real-time data to the fire centers, helping them make informed decisions. They can assign tasks to firefighters based on the fire's location and severity.

5. **Mobile App**: Firefighters receive their tasks and updates via a mobile app built using Flutter, which helps them respond quickly and efficiently.

---

## 6. System Components <a name="system-components"></a>
Each component of our system has its own dedicated README file:
- [Sensor Nodes](./SensorNode/README.md)
- [Gateway](./Gateway/README.md)
- [Backend Server](./BackendServer/README.md)
- [Dashboard](./Dashboard/README.md)
- [Mobile App](./MobileApp/README.md)

---

## 7. Block Diagram (DFD) <a name="block-diagram"></a>
The system follows a simplified Data Flow Diagram (DFD) to show the flow of data between components:

```
[Sensor Node] ---> [Gateway] ---> [Backend Server] ---> [Dashboard] ---> [Firefighters' Mobile App]
```

This diagram provides a high-level overview of how data flows from the forest to the firefighters.

---

## 8. Technology & Hardware Used <a name="technology--hardware-used"></a>
### Hardware:

- 2x ESP32 Microcontrollers
- DHT11 Temperature Sensor
- MQ9 Gas Sensor
- XL9006 Voltage Regulator
- TP4056 Battery Charging Module
- 5000mAh 3.7V Lithium Battery
- 2W Solar Panel
- Custom PCB Circuit
- 3D-printed components
- LED indicators, switches

### Software:
- Arduino IDE (C++)
- PHP & MySQL for backend server
- Symfony & Swagger for API development
- Flutter for mobile app and web dashboard development
- WordPress for the landing page

## 9. Results and Conclusion <a name="results-and-conclusion"></a>

By implementing Fireguard, we successfully showcased the potential of an IoT-based system in detecting forest fires early. The system efficiently monitors forest conditions, provides real-time data to fire stations, and assigns tasks to firefighters. While our prototype is focused on small-scale implementation, it has the potential to be expanded for larger areas.

## 10. Future Efforts <a name="future-efforts"></a>

For future development, we plan to:

- Improve sensor accuracy and coverage.
- Integrate AI algorithms for predictive analysis of fire outbreaks.
- Expand the system to handle larger forests and national parks.
- Collaborate with firefighting organizations to optimize response times.
- Develop a drone-based sensor system for faster deployment.

## 11. References <a name="references"></a>

- Syrian Ministry of Agriculture Fire Reports, 2022
- IoT-Based Forest Fire Detection Systems: A Survey, 2021
- LoRa Technology in IoT Networks, 2020

## 12. Credits <a name="credits"></a>

### Project Contributors:

- **Team Members**: [Obada Tarazi ,Mohammas al Hajjar , Mohammed al Dawaish ,Izzat Kawadri ]
- **Supervisors**: Professor [Sami AL Issa]
- **Special thanks to** [CupCoding ,StorageGuard Team,EVO Tech ].

We hope this project inspires others to explore the intersection of IoT and environmental conservation!
