# Air Sense & Weather Monitoring System

## Abstract
The Air Sense & Weather Monitoring System is a portable, low-cost, IoT-based
environmental monitoring solution designed to provide **real-time,
point-of-measurement environmental data**. Unlike conventional air quality and
weather monitoring applications that rely on **area-averaged values from
sparsely distributed monitoring stations**, this system captures environmental
parameters **directly at the location of deployment**, enabling accurate
micro-environmental assessment.

The system continuously measures temperature, humidity, atmospheric pressure,
altitude, ambient noise levels, and air quality. To ensure measurement
reliability and consistency, the prototype employs **industry-grade
environmental sensors** rather than hobby-grade modules, enabling improved
accuracy, stability, and repeatability suitable for real-world deployments.



This project was shortlisted among the **Top 17 prototypes out of 150+ submissions**
and secured **8th place** under the *Mentored Student Projects* category at
**IASF 2026 & ICTIEE 2026**, held at GITAM (Deemed to be University), Bengaluru.

---

## Motivation
Most existing air quality and weather monitoring platforms—including mobile
applications and government-operated monitoring stations—provide
**region-level or area-averaged environmental data**. While suitable for
macro-scale analysis, such data often fails to represent the **actual
environmental conditions experienced at a specific location**, particularly
within indoor environments, traffic-dense zones, industrial areas, and
noise-sensitive regions.

Furthermore, many low-cost monitoring solutions rely on **consumer- or
hobby-grade sensors**, which may suffer from poor accuracy, drift, and limited
long-term reliability.

The Air Sense & Weather Monitoring System addresses these limitations by enabling
**localized, point-of-measurement environmental sensing using industry-grade
sensors**, combined with standardized AQI computation. This approach delivers
accurate, reliable, and context-aware environmental insights for public health
awareness and early risk identification.

---

## System Overview
The system integrates multiple **industry-grade environmental sensors** with a
microcontroller-based embedded platform. Sensor data is sampled periodically,
processed locally, and displayed in real time on an OLED screen. The processed
data is also transmitted wirelessly to a cloud backend over Wi-Fi, allowing
users to access both real-time and historical environmental data through a
mobile application.

Unlike centralized monitoring stations that depend on spatial interpolation,
this system operates as a **distributed localized sensing node**, enabling
scalable deployment for high-resolution environmental monitoring.

The prototype is designed as a **dual-powered system**, capable of operating
both on **rechargeable battery power** and through an **external adapter-based
supply**. This dual-mode power architecture enables flexible deployment across
indoor and outdoor environments, ensuring uninterrupted operation during
mobility as well as long-duration stationary monitoring.


---

## Key Features
- Point-level environmental monitoring at the exact deployment location
- Use of **industry-grade sensors** for improved accuracy and stability
- Real-time sensing of multiple environmental parameters
- **Standardized AQI computation using CPCB (India) and AirNow (USA) methodologies**
- Local visualization using an OLED display
- Cloud connectivity via Wi-Fi
- Mobile application for remote monitoring and data access
- Portable, low-power, and modular system design
- Dual-powered operation using rechargeable batteries and external adapter supply


---

## Measured Parameters
- **Temperature**
- **Humidity**
- **Atmospheric Pressure**
- **Altitude**
- **Ambient Noise Levels**
- **Air Quality Index (AQI)**

---

## AQI Calculation Methodology
Air Quality Index values are computed from raw pollutant measurements using
**government-accepted AQI formulations**, ensuring regulatory relevance and
interpretability.

### AQI Standards Followed
- **CPCB (India)** AQI formulation based on sub-index calculation for individual
  pollutants and aggregation using the maximum sub-index approach.
- **AirNow (United States)** AQI methodology aligned with U.S. EPA standards for
  pollutant concentration-to-index mapping.
  
## Sources

- **National Air Quality Index (CPCB, India)**: https://cpcb.nic.in/National-Air-Quality-Index/
- **Air Quality Index (AirNow, U.S. EPA)**: [https://www.airnow.gov/aqi/](https://www.airnow.gov/aqi/aqi-basics/)



---


## Hardware Design
The hardware subsystem is designed with a focus on **measurement accuracy,
signal integrity, and deployment reliability**. It consists of:
- Industry-grade environmental sensors selected based on accuracy, operating
  range, and long-term stability
- A microcontroller unit for data acquisition and communication
- Signal conditioning and noise mitigation circuitry
- **Dual power supply architecture supporting both rechargeable battery
  operation and external adapter input**
- **Rechargeable battery pack enabling portable and uninterrupted operation**
- Power management circuitry optimized for efficiency, charging safety, and
  portable use


Component selection rationale, circuit diagrams, and hardware design
considerations are documented in the `hardware/` directory.

---

## Cloud & Mobile Application
The system supports cloud-based data logging and visualization:
- Structured JSON-based data transmission
- Cloud database for real-time and historical environmental records
- Mobile application for user-friendly visualization and monitoring

Cloud API design, database schema, and application architecture are documented
in the `cloud/` and `mobile_app/` directories respectively.

---

## Results & Performance
Experimental evaluation demonstrates:
- Stable and repeatable measurements across all parameters
- Reliable AQI estimation aligned with CPCB and AirNow standards
- Consistent wireless data transmission with low latency
- Effective capture of localized environmental variations not reflected in
  region-averaged data

Performance graphs, test cases, and result analysis are available in the
`results/` directory.

---


## Conference Recognition
- **Event:** IASF 2026 & ICTIEE 2026  
- **Category:** Mentored Student Projects  
- **Ranking:** 8th place  
- **Award:** ₹7,500 cash prize  

---

## Alignment with Sustainable Development Goals
This project aligns with **UN SDG 3 – Good Health and Well-Being** by enabling
localized environmental awareness and supporting early risk reduction through
continuous monitoring.


---

## Contributors
- Student Project Team  
- Mentors and Faculty Advisors  
- KLE Technological University  

---
For a detailed, chapter-wise technical study of the system, readers are
encouraged to refer to the project Wiki.
[https://github.com/<your-username>/Air-Sense-Weather-Monitoring-System/wiki](https://github.com/Sandeep-joshi123/Air-Sensing-and-Weather-Monitoring-System/wiki)


---

## Acknowledgments
We sincerely thank our mentors, KLE Technological University, and the organizers
of IASF 2026 & ICTIEE 2026 for their guidance, evaluation, and support throughout
this project.
