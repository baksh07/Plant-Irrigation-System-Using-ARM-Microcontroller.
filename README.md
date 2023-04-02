# Plant-Irrigation-System-Using-ARM-Microcontroller.
Firstly, we used an ARM microcontroller (LPC2148). We chose this microcontroller because of its high processing speed and low power consumption, making it suitable for embedded systems like plant irrigation.

We interfaced the microcontroller with a soil moisture sensor that we connected to the microcontroller's analog-to-digital converter (ADC) input. The sensor measures the soil moisture content and gives an analog output that is proportional to the soil moisture level. The microcontroller reads this output and uses it to determine the amount of water required by the plant.

To control the water pump, We used DC motor as reference to water pump. We connected it to one of the microcontroller's GPIO pins. The microcontroller sends a signal to the DC motor, which switches on or off as required.

We wrote the code for the system in embedded C language using the Keil uVision IDE. The code reads the sensor output and compares it with a predefined threshold value. If the soil moisture level falls below the threshold, the microcontroller sends a signal to the LCD, and with the help of external DC motor is turned ON. The DC motor runs until the moisture level reaches the desired value, and then it switches off.

