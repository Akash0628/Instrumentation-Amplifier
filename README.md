# Instrumentation-Amplifier
An instrumentation amplifier is a type of differential amplifier designed to amplify small differential signals while rejecting large common-mode voltages and noise. It is known for its high input impedance, low output impedance, and excellent common-mode rejection ratio (CMRR), making it ideal for precise and low-noise signal amplification. Typically, it consists of three operational amplifiers in a specific configuration: two op-amps in the first stage act as buffers with gain, while the third op-amp in the second stage functions as a differential amplifier. The gain of the instrumentation amplifier can be easily adjusted by changing a single external resistor, allowing for flexible amplification settings. Because of its accuracy and stability, the instrumentation amplifier is widely used in applications such as biomedical signal processing (e.g., ECG, EEG), sensor interfacing, and industrial process control, where small and sensitive signals need to be measured reliably in noisy environments.

### Design question:
Design an instrumentation amplifier using 3 op-amps configuration with the following constraints.
* R1=R2=R3=R4=R5=R6=100kΩ
* Difference gain Adm=20v/v
Find Acm and calculate CMRR for Adm=20v/v and 50v/v, by using LT spice simulator.

### Calculations:
For Adm=20v/v
Rg=[20000/19] =10.5kΩ
Rg=[20000/49] =4.08kΩ

## Circuit Diagram:

![image](https://github.com/user-attachments/assets/03659425-84e6-4f04-ad63-4be6def13f4a)
