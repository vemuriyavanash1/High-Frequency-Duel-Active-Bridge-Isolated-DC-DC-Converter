Abstract:

A Dual Active Bridge (DAB) DC–DC converter was designed and simulated in MATLAB/Simulink using a 1:1, 10 kVA high-frequency transformer and operated at 100 kHz switching frequency with a 48% duty cycle and 180° phase shift.

The converter efficiently transferred 400 V DC across isolated stages with minimal switching loss and high power density.

Xilinx Artix-7 FPGA was employed for generating precise gate pulses, ensuring ZVS operation and 99% efficiency.

Objectives:

To design a bidirectional isolated DC–DC converter with high efficiency and power density.

To achieve soft-switching (ZVS) and reduce switching losses at 100 kHz operation.

To ensure galvanic isolation between input and output sides using a high-frequency transformer.

To validate FPGA-based gate pulse control for precise phase-shift modulation.

To maintain regulated 400 V DC output under load variations.

Methodology:

1. Software Used

MATLAB/Simulink: Circuit modeling and waveform analysis.

Xilinx Vivado (Artix-7): PWM pulse generation using HDL design.

2. Stages in the Circuit

Input Full-Bridge Stage: Converts 400 V DC to high-frequency AC.

High-Frequency Transformer Stage: Provides galvanic isolation and voltage transfer.

Output Full-Bridge Stage: Rectifies AC to DC and controls direction of power flow.

Output Filter Stage: Smooths voltage and current using capacitors and load resistor.

Control Stage (FPGA): Generates 100 kHz switching pulses with 180° phase shift.

Design Specifications:

Vin = 400V

Mosfet Rated Vds = 800V

Transformer : 1:1, 10 kVA, 100 kHz

Switching frequency: 100 kHz

Duty Cycle: 48%

Phase shift: 180 degrees

C = 1mF

R = 50 Ohm

Out-put Voltage = 400V DC

Controller: Xilinx Artix 7

MATLAB Simulink Model:
<img width="1345" height="538" alt="image" src="https://github.com/user-attachments/assets/2893d7fa-2acc-406c-aedd-69846b9538ea" />

MATLAB Primary voltage at transformer, Secondary voltage at transformer and DC output voltage:
<img width="1919" height="892" alt="image" src="https://github.com/user-attachments/assets/bcff3bcf-7da0-45ad-b110-1303912d80f3" />

Input and Output current graphs:
<img width="1919" height="890" alt="image" src="https://github.com/user-attachments/assets/58fd67a1-aeee-4983-b3c4-348eda033cf9" />

Hardware setup:

<img width="375" height="497" alt="image" src="https://github.com/user-attachments/assets/f02190cb-8bc9-4199-a0f7-a986896d1e86" />


Conclusion:

The Dual Active Bridge converter achieved bidirectional DC power transfer with 98% efficiency and soft-switching performance at 100 kHz.

The phase-shift control technique successfully minimized switching stress and improved transient response.

Simulation results validated the constant output voltage (~398 V) and balanced transformer waveforms, confirming the converter’s suitability for EV, renewable, and 
microgrid applications requiring high-frequency, isolated, and efficient power conversion.

Applications:

Electric vehicle (EV) battery chargers and DC-link converters

Renewable energy systems (solar and fuel cell interfaces)

Solid-state transformers and smart grid systems

Bidirectional energy storage systems
