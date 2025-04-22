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

![image](https://github.com/user-attachments/assets/d0ea4c66-618e-42f0-8220-67864dff4f34)


#### For Adm=20v/v

![WhatsApp Image 2025-04-22 at 15 41 31_f16f3a93](https://github.com/user-attachments/assets/5521480a-45d6-4fc8-b554-4efdc07f3fbf)

from above output we get vout=0.9*10^-9

Acm=vout/vin 

Acm=9*10^-9

CMRR=20log(Adm/Acm) 

CMRR=186.93dB

#### For Adm=50v/v

![WhatsApp Image 2025-04-22 at 15 50 37_0365e1bf](https://github.com/user-attachments/assets/252a539f-98e6-479b-918c-c457d74455b4)

from above output we get vout=0.9*10^-9

Acm=vout/vin 

Acm=9*10^-9

CMRR=20log(Adm/Acm) 

CMRR=194.8dB

### Result:
for Adm=20v/v, get the CMRR as 186.93dB and for Adm=50v/v, get the CMRR as 194.8dB

### Inference:

The simulation of the instrumentation amplifier using an ADM-series IC in LTspice demonstrates effective differential signal amplification with high common-mode noise rejection. The output accurately reflects the amplified difference between the input signals, validating the circuit’s performance in low-noise, precision applications. The gain of the amplifier responds correctly to changes in the external gain-setting resistor, confirming its predictable and stable behavior. The high input impedance and excellent common-mode rejection observed in the simulation align with theoretical expectations, making the configuration suitable for applications such as sensor signal conditioning and biomedical instrumentation.

Adm=[1+2Rs/Rg]8R2/R1 used to find Rgb in this.

