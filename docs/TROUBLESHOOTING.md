# Troubleshooting and engineering observations

**Source:** Original 39-page CEIS114 academic presentation by Mildred Owens, particularly pages 34–36.  
**Context:** ESP32-based IoT traffic-control simulation, with physical circuitry, Arduino IDE, LCD, and buzzer.

## Case 1: ESP32 serial connection not detected
**Observed problem:** Arduino IDE did not expose a usable communication port on either the MacBook Pro or a Windows 10 computer.

**Diagnostics performed:** Checked the USB connection, replaced the kit's cable with another included cable, reinstalled drivers, and compared findings with classmates who experienced the same issue.

**Resolution recorded:** A separate micro-USB cable previously used with a tablet allowed communication. The ESP32's reboot button was also used during connection.

**Engineering lesson:** Power delivery from a USB cable does not prove that the cable can transmit data. Test the physical link before continuing to alter software configuration.

## Case 2: Red LED response to pedestrian button
**Observed problem:** Two red LEDs did not respond as expected to the tactile push button.

**Diagnostics performed:** Inspected breadboard placement and wire alignment; checked continuity using a multimeter; identified three non-working switches and two faulty wires in the available kit.

**Resolution recorded:** Replaced faulty parts, adjusted wiring placement, and held the button through the programmed LED cycle until the intended response was observed.

**Technical limitation:** A standard normally-open momentary switch is closed while pressed and opens when released. The reported multi-second delay may have come from firmware logic, input polling, debounce behavior, or the traffic-light sequence. The archived evidence does not isolate which explanation was responsible.

## Case 3: Buzzer produced an unexpected intermittent sound
**Observed problem:** The expected continuous warning sound was intermittent or pulsing during part of the countdown.

**Diagnostics performed:** Checked wiring and compared the buzzer's pins with the breadboard orientation and instructional material.

**Resolution recorded:** Corrected the buzzer connections; the demonstration subsequently produced the expected warning indication.

## Verification sources
The original presentation contains photographs of the physical build, Arduino IDE code screenshots, Serial Monitor outputs, and a step-by-step account of troubleshooting. The linked demonstration shows the circuit operating.

[View the project demonstration](https://youtu.be/fZm6KXImiJk)

**Important:** This document preserves the author's original observed results but does not claim independent electrical verification, a security audit, or safety certification.
