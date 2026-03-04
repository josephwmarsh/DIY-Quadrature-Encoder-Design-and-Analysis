
# DIY Quadrature Encoder and Motor Control System
### Physical Signal Processing and Mechatronic Integration

## Project Overview
This project involves the ground-up design and implementation of a 2-channel quadrature encoder used to track the rotational position and direction of a motor shaft. Unlike commercial optical encoders, this system utilizes a custom-patterned encoder disc and photoresistors (LDRs) to demonstrate the fundamental principles of quadrature encoding, signal phase shifts, and closed-loop control.

## Technical Specifications
* **Sensor Type:** Dual-channel Photoresistor (LDR) array.
* **Encoding Logic:** 2-channel Quadrature (A and B signals) for direction sensing and position tracking.
* **Control Platform:** Arduino Microcontroller.
* **Actuation:** Integrated DC motor controlled via encoder feedback loops.
* **Mechanism:** Concentric encoder disc featuring alternating transparent and opaque segments to generate pulsed signals.



## Engineering Challenges and Solutions
### Signal Phase Alignment
To achieve directional sensing, the sensors were physically positioned to generate a 90-degree phase shift between Channel A and Channel B.
* **Clockwise (CW):** Channel A leads Channel B.
* **Counter-Clockwise (CCW):** Channel B leads Channel A.

### Robust Signal Processing
Because LDRs produce analog voltage fluctuations rather than clean digital pulses, I implemented threshold-based logic in the software to convert analog inputs into stable digital states, mitigating noise from ambient light interference.

## Results and Impact
* **Functional Validation:** Successfully tracked motor position in real-time, allowing for precise angular control.
* **Educational Scalability:** Designed the system using accessible materials (cardboard, basic electronics) to serve as a high-level demonstration of encoder physics for educational purposes.
* **Technical Growth:** Gained deep experience in hardware-software synchronization and the importance of pre-project systems mapping.
