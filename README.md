
# Exp 4 Experimental verification of frequency response of Analog fiber optic link
# Fiber Optic Link Analysis (660nm)

## AIM:
To analyze the relationship between input and received signal of a 660nm fiber optic cable using analog and digital link.

---

## EQUIPMENTS REQUIRED:
- Fiber optic trainer kit ST 2502  
- Power supply  
- Patch cords  
- CRO (Cathode Ray Oscilloscope)  
- 660 nm fiber cable  

---

## THEORY:
Fiber optic links can be used for transmission of digital as well as analog signals. Basically a fiber optic link contains three main elements, a transmitter, an optical fiber and a receiver. The transmitter module takes the input signal in electrical form and then transforms it into optical (light) energy containing the same information. The optical fiber is the medium which takes the energy to the receiver. At the receiver light is converted back into electrical form with the same pattern as originally fed to the transmitter.

TRANSMITTER: Fiber Optic transmitters are typically composed of a buffer, driver and Optical Source. The buffer electronics provides both an electrical connection and isolation between the transmitter and the electrical system supplying the data. The driver electronics provides electrical power to the Optical source in a fashion that duplicates the pattern of data being fed to the transmitter. Finally the optical source (LED) converts the electrical current to light energy with the same pattern. The LED SFH450V (950nm) supplied with this kit operates outside the visible light spectrum. Its Optical output is centered at near infrared wavelength of 950nm. The LED SFH756V (660nm) supplied with this kit operates at the visible light spectrum. Its Optical output is centered at wavelength of 660nm.

RECEIVER: The function of the receiver is to convert the optical energy into electrical form, which is then conditioned to reproduce the transmitted electrical signal in it's original form. The detector SFH350V (Photo Transistor Detector) used in the kit has a transistor type output. The parameters usually considered in the case of detector are it's responsivity at peak wavelength and response time. SFH350V (Photo Transistor Detector) has responsivity of about 0.8mA/10uW at 660nm. But its response time is quite large and thus has lower bandwidth of about 300 KHz. When optical signal falls on the base of the transistor detector, proportional

current flows through its emitter generating the voltage across the resistance connected between emitter and ground. This voltage is the duplication of the transmitted electrical signal, which can be amplified.

---

## PROCEDURE:

1. Connect the power supply to the board.  
2. Ensure that all switched faults are set to ‘Off’.  
3. Make the following connections (as shown in Figure 19):  
   a. Connect the 1KHz sine wave output to emitter 1's input.  
   b. Connect the fiber optic cable between emitter output and detector input.  
   c. Connect detector 1's output to AC amplifier 1 input.  
4. On the board, switch emitter 1's driver to analog mode.  
5. Switch on the power.  
6. Observe the input to emitter 1 (TP5) and the output from AC amplifier 1 (TP28). Verify that both signals are identical.  
7. Vary the frequency between 10 Hz to 1 MHz and observe the output voltage for a constant input voltage of 5V.  
8. Calculate the bandwidth by determining the gain in decibels (dB).  

---

## BLOCK DIAGRAM:
<img width="433" height="258" alt="image" src="https://github.com/user-attachments/assets/d7782ce0-f79e-4def-a5bb-29cee0dd91fe" />

## TABULATION:
**Transmission through Analog Link**

| Frequency (Hz) | Output Signal Amplitude (Vo) | Gain = Vo/Vi | Gain in dB |
|----------------|------------------------------|--------------|------------|
|      800       |           120 mV             |    0.024     |  -32.395   |
|      1.5k      |           216 mV             |    0.0432    |  -27.290   |
|      3k        |           412 mV             |    0.134     |  -21.681   |
|      5k        |           670 mV             |    0.1848    |  -17.457   |
|      7k        |           924 mV             |    0.19      |  -14.665   |
|      9k        |           950 mV             |    0.19      |  -14.424   |
|      11k       |           950 mV             |    0.19      |  -14.424   |
|      13k       |           950 mV             |    0.19      |  -14.424   |
|      15k       |           950 mV             |    0.19      |  -14.424   |
|      50k       |           840 mV             |    0.168     |  -15.493   |
|      200k      |           385 mV             |    0.077     |  -22.270   |
|      600k      |           280 mV             |    0.056     |  -25.036   |
|      800k      |           95 mV              |    0.19      |  -34.424   |
|      1M        |           58 mV              |    0.011     |  -39.172   |

## MODEL GRAPH:
<img width="487" height="220" alt="image" src="https://github.com/user-attachments/assets/f3072b68-a9fd-4112-b3b7-8b3d8fab1d42" />

## GRAPH:
![WhatsApp Image 2025-11-16 at 21 59 45_135f009c](https://github.com/user-attachments/assets/62d903b1-19b5-4197-93b4-a1f4036e6c8b)


## RESULT:
Thus, the frequency response of the analog fiber optic link was successfully studied, and the bandwidth was determined to be 95 kHz.
---
