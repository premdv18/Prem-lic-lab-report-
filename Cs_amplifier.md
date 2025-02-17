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
AC gain depends on transconductance (gm) and resistors. A larger W/L ratio increases gm and boosts gain.


2. DC Bias Point:
Bias point is influenced by V_GS and V_DS. W/L changes affect the operating point and stability.


3. Transient Analysis:
Transient response is affected by W/L, with a larger ratio improving signal handling and reducing distortion.




Changing the MOSFET’s width (W) and length (L) will directly influence these parameters. A larger W results in higher transconductance (gm), improving the gain and transient response, while a smaller L helps reduce channel length modulation, stabilizing the bias point.

