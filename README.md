# ESP32 IoT Traffic Control System

**Academic Project | DeVry University, CEIS114 Introduction to Digital Devices**  
**Project author:** Mildred Owens

## Project overview
An ESP32-based Internet of Things (IoT) traffic-control prototype developed through a series of hands-on academic modules. The project demonstrates how hardware, embedded programming, networking, user input, and cloud-based commands can interact in a single device.

The prototype evolved from a basic red-yellow-green LED sequence to a multiple-light simulation with pedestrian-crossing input, an LCD countdown, an audible buzzer, and an emergency indicator controlled through an IoT web interface.

## Features demonstrated
- ESP32 microcontroller driving two sets of traffic lights.
- Red, yellow, and green LED traffic sequences.
- Momentary tactile-button pedestrian-crossing input.
- Serial Monitor output for **Do Not Walk** and a walk countdown.
- LCD display and buzzer integration.
- Blue LED emergency indication and cloud-based control, demonstrated using the Cayenne IoT service.
- ESP32 Wi-Fi scanning and Arduino IDE serial-port configuration.

This is an **educational simulation**, not a traffic-safety-certified controller or a production IoT deployment.

## Engineering process
The work was developed incrementally: component inventory and ESP32 setup, initial LED cycling, dual signal sets, push-button pedestrian logic, LCD/buzzer integration, and IoT-enabled emergency control.

### Troubleshooting case studies
**1. ESP32 not detected by Arduino IDE**  
The microcontroller did not present a serial port on either macOS or Windows. After checking connections, trying bundled cables and reinstalling drivers, a different micro-USB data cable allowed successful communication.

**2. Pedestrian push button did not trigger red LEDs as expected**  
Breadboard placement and wiring were checked; multimeter continuity tests identified defective switches and two faulty wires. Replacement components and a sustained press allowed the project to demonstrate the expected LED sequence. The exact cause of the observed delay was not independently isolated.

**3. Buzzer produced an unexpected intermittent sound**  
The buzzer connections and pin orientation were reviewed and corrected. The subsequent demonstration produced the intended warning indication.

These examples show a practical workflow of observing a fault, testing possible causes, changing components or connections, and checking behavior again.

## Demonstration
[Watch the traffic-control demonstration on YouTube](https://youtu.be/fZm6KXImiJk)

## Evidence and documentation
The original course presentation documents the module progression, circuit photographs, Arduino IDE screenshots, serial output, and troubleshooting notes. A shareable, sanitized version of the 39-page presentation can be added here after removing historical connection strings and credentials from screenshots. Project photographs and recordings are original academic work.

## Skills illustrated
**ESP32 and IoT fundamentals · hardware/software integration · Arduino IDE · GPIO and digital I/O · Wi-Fi concepts · functional testing · multimeter-based diagnostics · technical troubleshooting · engineering documentation**

## Scope and authorship
This repository documents **Mildred Owens's academic hardware and IoT project** and her original troubleshooting observations. It should not be interpreted as an independently security-audited cloud service or as evidence of production-grade traffic signaling.

## Relationship to later work
The project helped build an early foundation in systems thinking, component integration, troubleshooting, and evidence-based validation. Those approaches continued to inform later cybersecurity studies and the independent CIPHER AI systems project.
