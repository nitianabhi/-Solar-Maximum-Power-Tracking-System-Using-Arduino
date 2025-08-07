# Servo Motor Control Using LDRs

This project controls the position of a servo motor based on the light intensity detected by two LDR (Light Dependent Resistor) sensors. It automatically adjusts the servo to track the brighter light source.

---

##  Theory of this Project

The project is based on the principle of a light-following mechanism:
- Two LDRs are placed such that they sense light from different directions.
- The difference in light intensity from the two LDRs is measured.
- Depending on which side is brighter, the servo motor rotates to align with the light.

### Theory in Images:
<img width="614" height="800" alt="Image" src="https://github.com/user-attachments/assets/33aa047b-ae23-4adc-aa9a-bbb48a06c245" />
*Light sensing using LDRs.*

<img width="718" height="843" alt="Image" src="https://github.com/user-attachments/assets/132777bc-d4a9-4f5b-8300-bd9c6d4bbf19" />
*Error calculation based on the difference in LDR readings.*

<img width="719" height="482" alt="Image" src="https://github.com/user-attachments/assets/e223dacf-0d7e-4e02-96f2-dcff1dfcae0b" />
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
<img width="698" height="798" alt="Image" src="https://github.com/user-attachments/assets/2568071b-af66-418c-9e1a-4df5bb213771" />
*All electronic components.*

<img width="719" height="212" alt="Image" src="https://github.com/user-attachments/assets/2eaaee0b-c326-44ea-bdf5-fa4099c31cd9" />
*Close-up of the servo and LDRs.*

---

## 🔗 Connections & Circuit

The two LDRs are connected to the analog pins of the Arduino. A voltage divider is used with each LDR to provide a measurable voltage. The servo motor signal wire is connected to a PWM-capable digital pin.

### Circuit in Images:
<img width="783" height="426" alt="Image" src="https://github.com/user-attachments/assets/11ad8f74-a729-419e-990a-362ce7e8884b" />
*Wiring diagram of the setup.*

<img width="659" height="570" alt="Image" src="https://github.com/user-attachments/assets/b58e3609-8b0d-408e-b8c3-c2893fa06c57" />
*Breadboard connection of the circuit.*

<img width="716" height="800" alt="Image" src="https://github.com/user-attachments/assets/e0f2dfe6-fac1-4bff-9398-e46b3fc1e3dc" />

<img width="708" height="483" alt="Image" src="https://github.com/user-attachments/assets/21b5bc04-f884-49b2-a8a0-bfd06bab54b7" />
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


