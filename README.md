# Smart Accident Detection & Location Tracking System

> An academic Electronic Lab project exploring IoT-based accident
> alerts, GPS location sharing, and driver drowsiness monitoring.

**Project status:** Prototype development / planned rebuild\
**Demo video:** Not currently available\
**Last updated:** November 2026

## 1. Project Overview

This project explores a prototype that can detect a possible
road-accident event and share its location with a designated contact. It
also explores driver drowsiness monitoring using a camera-based
eye-detection approach.

The project was developed as an academic Electronic Lab project. The
physical prototype was assembled for demonstration, but it has since
been dismantled. The project will be rebuilt and tested again before any
final performance claims are made.

## 2. Project Objectives

-   Explore motion-sensor-based detection of a possible accident event.
-   Obtain location information from a GPS module.
-   Demonstrate how an alert could be sent using a communication module
    or an internet-based messaging service.
-   Explore camera-based eye-state detection as a driver-drowsiness
    warning feature.
-   Present the system as a small-scale educational prototype.

## 3. Proposed System Architecture

The intended prototype is divided into these functional parts:

1.  **Motion sensing:** An MPU6050 sensor provides motion and
    acceleration readings for detecting unusual movement.
2.  **Controller:** An Arduino or ESP32-based controller processes
    sensor readings and coordinates the prototype.
3.  **Location tracking:** A NEO-6M GPS module provides location
    coordinates.
4.  **Alert communication:** A GSM module or an internet-connected ESP32
    can be used to send a notification.
5.  **Drowsiness monitoring:** An ESP32-CAM-based camera module explores
    eye-state detection using a machine-learning model.
6.  **Demonstration output:** LEDs and a buzzer provide local status
    indications. Any relay-based control is intended only for a
    low-voltage tabletop or RC-car demonstration.

## 4. Hardware Considered

The following components were considered for the academic prototype. The
final component list and wiring will be confirmed during the rebuild.

-   Arduino UNO / Nano or ESP32 development board
-   ESP32-CAM
-   MPU6050 (GY-521) motion sensor
-   NEO-6M GPS module
-   SIM800L / SIM7600 GSM module, or Wi-Fi-based messaging
-   Buzzer and status LEDs
-   Push button for acknowledgement/reset
-   Relay or motor-driver module for a low-voltage RC-car demonstration
-   Suitable regulated power supplies and connecting wires

## 5. Software and Technologies

-   Arduino IDE
-   Embedded C/C++ (Arduino sketches)
-   ESP32 camera support
-   GPS data parsing
-   GSM or Wi-Fi-based notification
-   Edge Impulse / machine-learning-based eye-state detection (planned
    for re-testing)

## 6. Intended Working Flow

### Possible accident alert

1.  The motion sensor continuously provides readings to the controller.
2.  The controller checks whether the readings indicate an unusual
    event.
3.  If a possible event is detected, the prototype provides a local
    warning using an LED and buzzer.
4.  The GPS module is used to obtain coordinates.
5.  The communication module can send an alert containing the available
    location information.

### Driver drowsiness monitoring

1.  The camera captures images of the driver's eye area in a controlled
    demonstration.
2.  The eye-detection model estimates whether the eyes appear open or
    closed.
3.  The prototype can provide a warning when the configured drowsiness
    condition is detected.

These are the intended functions. Detection accuracy, timing, and
end-to-end operation must be re-tested and documented after the
prototype is rebuilt.

## 7. Current Project Status

  Item                           Current status
  ------------------------------ ------------------------------------------------
  Academic project concept       Defined
  Hardware prototype             Previously assembled; currently dismantled
  Source code                    Needs to be collected, reviewed, and organized
  Circuit diagram                Needs to be recreated and verified
  Accident-detection testing     Needs to be repeated
  GPS and notification testing   Needs to be repeated
  Camera-based eye detection     Needs to be re-tested
  Demo video                     Not available
  Rebuild and documentation      Planned

## 8. Limitations and Safety

-   This is an educational prototype, not a certified vehicle-safety
    device.
-   Sensor thresholds alone cannot reliably determine whether a real
    road accident has occurred.
-   GPS reception and message delivery may be delayed or unavailable.
-   Camera-based eye detection can be affected by lighting, camera
    position, and model accuracy.
-   Any motor or relay demonstration must remain limited to a
    low-voltage RC car or tabletop setup. Do not connect this prototype
    to a real vehicle's engine or safety systems.
-   The system must not be relied on for emergency response or
    real-world driving decisions.

## 9. Planned Improvements

-   Rebuild the prototype and verify each module separately.
-   Recreate and document the actual circuit connections.
-   Test the motion-sensor logic under controlled, safe conditions.
-   Verify GPS coordinates and notification delivery.
-   Re-test the eye-detection model and record its limitations.
-   Add genuine prototype photographs and a short demonstration video
    after rebuilding.
-   Update this repository with tested source code and results.

## 10. Repository Structure

The repository will be organized as the project is rebuilt:

``` text
Smart-Accident-Detection-System/
├── README.md
├── Code/
│   ├── Arduino/
│   ├── ESP32/
│   └── ESP32_CAM/
├── Documentation/
│   └── Circuit_Diagram/
└── Images/
```

Folders can be added when the corresponding files are ready.

## 11. Developer

**Sohel Khan**\
GitHub: [SkCaCo3](https://github.com/SkCaCo3)

------------------------------------------------------------------------

*This README is an initial project overview. It will be updated with
verified circuit diagrams, source code, photographs, and test results
after the prototype is rebuilt.*
