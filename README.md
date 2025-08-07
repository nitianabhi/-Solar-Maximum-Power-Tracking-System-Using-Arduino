# Servo Motor Control Using LDRs

This project controls the position of a servo motor based on the light intensity detected by two LDR (Light Dependent Resistor) sensors. It automatically adjusts the servo to track the brighter light source.

---

##  Theory of this Project

The project is based on the principle of a light-following mechanism:
- Two LDRs are placed such that they sense light from different directions.
- The difference in light intensity from the two LDRs is measured.
- Depending on which side is brighter, the servo motor rotates to align with the light.

### Theory in Images:
![Theory 1](images/theory1.png)
*Light sensing using LDRs.*

![Theory 2](images/theory2.png)
*Error calculation based on the difference in LDR readings.*

![Theory 3](images/theory3.png)
*Servo adjusts its position according to the light direction.*

---

##  Components Used

- 1 × Arduino board
- 1 × Servo motor
- 2 × LDR sensors
- 2 × Resistors (10kΩ, for voltage divider)
- Breadboard and jumper wires
- Power supply

### Components in Images:
![Components 1](images/components1.png)
*All electronic components.*

![Components 2](images/components2.png)
*Close-up of the servo and LDRs.*

---

## 🔗 Connections & Circuit

The two LDRs are connected to the analog pins of the Arduino. A voltage divider is used with each LDR to provide a measurable voltage. The servo motor signal wire is connected to a PWM-capable digital pin.

### Circuit in Images:
![Circuit 1](images/connection1.png)
*Wiring diagram of the setup.*

![Circuit 2](images/connection2.png)
*Breadboard connection of the circuit.*

![Circuit 3](images/connection3.png)

![Circuit 4](images/connection4.png)
---

##  How the Code Works

- The Arduino continuously reads analog values from the east and west LDRs.
- If the difference between them exceeds a threshold, the servo motor rotates towards the brighter side.
- The servo stops when the difference falls below the threshold.

### Code in Images:
![Code 1](images/codeworks1.png)
*Reading LDR values and calculating error.*

![Code 2](images/code2.png)
*Controlling servo position based on error.*

---

## Conclusion

The Solar Maximum Power Tracking System effectively demonstrated how solar energy efficiency can be enhanced using a simple Arduino-based sun-tracking mechanism. By automatically adjusting the panel's orientation based on real-time light intensity from LDR sensors, the system ensures maximum exposure to sunlight throughout the day. This project highlights the potential of embedded systems and renewable energy integration, offering a scalable solution for energy optimization in both small-scale and commercial solar applications.

---


