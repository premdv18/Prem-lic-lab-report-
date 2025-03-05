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

## DC Analysis 

## Transient Analysis 

## AC Analysis 

## 2.Circuit 2(Common Source terminal is connected with current source):
In this configuration, an ideal current source replaces the resistor at the common source node. The sources of M1 and M2 are connected to this current source (Iss). The rest of the circuit remains the same.

## DC Analysis 

## Transient Analysis 

## AC Analysis 

## 3.Circuit 3(Common Source terminal is connected with MOSFET):
In this configuration, a MOSFET (M3) is used instead of a current source. The sources of M1 and M2 are connected to the drain of M3, whose source is grounded.The rest of the circuit follows the same design.

## DC Analysis 

## Transient Analysis 

## AC Analysis 






