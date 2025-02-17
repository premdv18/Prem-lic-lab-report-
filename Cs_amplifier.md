## Aim 

To create and simulate a Common Source (CS) Amplifier with LTspice and evaluate its performance by DC Analysis, AC Analysis, and Transient Analysis to observe its gain, frequency response, and transient response.

## Components required 

1. Power Supply: 1.8V, 0.9V
2. Resistors: 1kΩ
3. NMOS Transistor
4. PMOS Transistor
5. Connecting Wires

## Theory

MOSFET (Metal-Oxide-Semiconductor Field-Effect Transistor) is a voltage-controlled device used for switching and amplification. It has three terminals: Gate (G), Drain (D), and Source (S). MOSFETs are classified into NMOS and PMOS types.

Modes of Operation of MOSFETs
1. Cutoff Region  
2. Triode (Linear) Region  
3. Saturation (Active)
   we can calculate drain current using the below equation for mosfet in active region 
   I_D = (1/2) * μ_n * C_ox * (W/L) * (V_GS - V_TH)²
# Types of Analysis

1. DC Analysis – Determines the operating point of the circuit.  
2. AC Analysis – Evaluates frequency response and gain.  
3. Transient Analysis – Studies time-domain behavior of the circuit.

## Procedure 
1. Create the circuit by placing and connecting components like resistors, capacitors, transistors, and voltage sources according to your design.


2. For DC Analysis, click Simulate, Edit Simulation Cmd and select .DC to analyze the operating point of the circuit.


3. For AC Analysis, click Simulate, Edit Simulation Cmd and select .AC DEC 20 .1 1T to analyze the frequency response of the circuit.


4. For Transient Analysis, click Simulate, Edit Simulation Cmd and select .TRAN 3m to simulate the time-domain behavior of the circuit.


5. Run the simulation by pressing the Run button, and LTspice will display the results.


6. View the results by clicking on nodes or components to see voltage or current waveforms and adjust the time scale or plot other parameters for analysis.


7. Save and analyze the schematic and waveform for future reference or adjustments.
## Circuit 

## Calculation

## DC Analysis 

## AC Analysis 

## Transient Analysis 

## Inference

1. AC Gain:
The AC gain of a CS amplifier is determined by the values of resistors (RD, RL) and the transistor parameters (such as the transconductance gm). The AC gain can be approximated as:
A_v ≈ -gm * RD
Changing the width (W) and length (L) of the MOSFET affects the transconductance (gm), thus influencing the gain. A larger W/L ratio typically increases gm and, consequently, the AC gain.


2. DC Bias Point:
The DC bias point is set by the gate-source voltage (V_GS) and the drain-source voltage (V_DS). In a CS amplifier, the MOSFET operates in the saturation region under normal conditions. The biasing can be adjusted using resistors and the power supply voltage. Changes in W/L will affect the MOSFET's threshold voltage and operating point, which might shift the bias point. For a stable DC bias point, the correct selection of W/L ratio and external biasing resistors is essential.

3. Transient Analysis:
Transient analysis shows the time-domain response of the amplifier, typically showing the amplifier’s behavior when subjected to an input signal. The response is influenced by the MOSFET's intrinsic capacitances, the values of resistors, and the coupling capacitors. As the W/L ratio of the MOSFET increases, the overall current drive capability increases, affecting the rise and fall times in the transient response. A larger W/L ratio improves the device's ability to handle larger signals with faster transitions, reducing distortion in the transient response.


Changing the MOSFET’s width (W) and length (L) will directly influence these parameters. A larger W results in higher transconductance (gm), improving the gain and transient response, while a smaller L helps reduce channel length modulation, stabilizing the bias point.

