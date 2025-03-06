# Experiment 3

## Differential Amplifier 

## Aim

To simulate a differential amplifier using LTspice and analyze its performance through AC, DC, and Transient analysis. The objective is to study the amplifier's gain and frequency response.

## Theory 

A differential amplifier is a circuit that amplifies the difference between two input signals while rejecting common-mode signals. It is widely used in analog signal processing and operational amplifiers.

A basic differential amplifier consists of two identical MOSFETs with a common current source. The inputs are applied to the gates, and the output is taken as the difference between the two drain voltages.


This experiment is conducted in three stages.Where common source terminal is connected with 

1. Resistor
2. Current source
3. MOSFET


### To conduct we need to solve the given question.
P=2.2mW

By solving

Iss=P/V=2.2mW/2.2=1mA

RD=VDD-Vocm/ID1=2.2-1.25/0.5*10^-3=1.9kohm

ID1=ID2=Iss/2=1mA/2=0.5mA

Rss=Vp/Iss=0.4/1*10^-3=400ohm

## 1.Circuit 1(Common Source terminal is connected with resistor):
In this configuration, a resistor is used at the common source node. Two identical MOSFETs (M1 and M2) have their sources connected to a single resistor (Rss), which is then grounded. The drains of both MOSFETs are connected to the power supply (VDD) through load resistors (RD). The inputs are applied to the gates of M1 and M2, and the output is taken as the voltage difference between their drains.

## Circuit
![17412477711125548294441902748008](https://github.com/user-attachments/assets/0c9114c2-9494-42ef-a962-738bd61ff832)


## DC Analysis 
![17412475110018964593564396166929](https://github.com/user-attachments/assets/0f159ec7-d6ac-4756-bcf4-7b72c5ab4c98)


## Transient Analysis 
![17412476015052674709694416888091](https://github.com/user-attachments/assets/fefce5f5-19e7-428b-a122-ccefa9dab510)

Voltage gain(Av) = vout/vin
            =(1.322-1.1766)/(1.2493-1.159)
            =1.470V/V
 Voltage gain of MOSFET is 1.470V/V


## AC Analysis 
![17412476527696928533782234646353](https://github.com/user-attachments/assets/51933e9e-5359-4303-8f39-5aae02382887)

Gain = 3.346dB




## 2.Circuit 2(Common Source terminal is connected with current source):
In this configuration, an ideal current source replaces the resistor at the common source node. The sources of M1 and M2 are connected to this current source (Iss). The rest of the circuit remains the same.

## Circuit
![17412478321166600532936376382052](https://github.com/user-attachments/assets/ffbb77c9-5aa6-4cbe-b485-946b3e70f28c)


## DC Analysis 
![17412479921571770524406942182331](https://github.com/user-attachments/assets/87e7365d-8991-4f72-87e9-509bf9fc3af7)


## Transient Analysis 
![17412481588121129465061794496593](https://github.com/user-attachments/assets/d406e63c-4732-4c5c-bd32-254dd8bbb7f8)

Voltage gain(Av) = vout/vin
            =(1.449-1.049)/(1.250-1.149)
            =3.9603V/V
 Voltage gain of MOSFET is 3.9603V/V


## AC Analysis 
![17412485092421809594723911609924](https://github.com/user-attachments/assets/70c8ffd0-ff70-44a7-a2c2-0639f1de38e4)

Gain = 11.95dB


## 3.Circuit 3(Common Source terminal is connected with MOSFET):
In this configuration, a MOSFET (M3) is used instead of a current source. The sources of M1 and M2 are connected to the drain of M3, whose source is grounded.The rest of the circuit follows the same design.

## Circuit
![17412485861052173336423909742662](https://github.com/user-attachments/assets/7cd41a00-6df5-4d69-bea4-7fd3fe75f4dc)


## DC Analysis 
![17412486682339190977595657264391](https://github.com/user-attachments/assets/e2d701eb-1260-4d1c-ab3e-349f0041408b)


## Transient Analysis 
![17412487578465120185144327858897](https://github.com/user-attachments/assets/e931d206-fdfa-4616-9c25-83ee9b264a80)

Voltage gain(Av) = vout/vin
            =(1.4469-1.047)/(1.2517-1.1486)
            =3.8787V/V
 Voltage gain of MOSFET is 3.8787V/V

## AC Analysis 
![1741248809543256303583399101819](https://github.com/user-attachments/assets/2567b3c3-64a6-45ff-80a8-59af52e93267)

Gain = 11.77dB

## Inference
 
 When using a resistor at the common source, the circuit is simple but not very stable. The gain changes with power supply variations, and the common-mode rejection is not very good.  

Replacing the resistor with an ideal current source improves the circuit significantly. The gain becomes more stable, and the common-mode rejection is much better. However, generating an ideal current source requires extra circuitry.  

Using a MOSFET as a current source gives the best performance. It provides high gain, excellent common-mode rejection, and better stability. This makes it the best choice for applications that need precision.  






