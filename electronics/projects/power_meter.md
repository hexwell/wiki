# Power meter

This project consist of a current transform connected to an arduino via a shunt resistor. The transformer is attached to one of the master live wire in my house and the arduino senses the voltage on the resistor in order to calculate the current power usage.

</br>

Considerations:
- For this project one could use an oscilloscope to better see the waveform of the current picked up by the transformer.
- In order to calculate correctly the power usage I must know the power factor of the load.
- Measuring the voltage as well might help with the accuracy of the measurement as well. This may be related to the power factor but it requires further investigation on my part.
