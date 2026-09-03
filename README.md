# DC-DC Boost Converter — Design & Closed-Loop Simulation

A 5V-to-12V boost converter designed and simulated for closed-loop steady-state voltage regulation, with a custom KiCad schematic and PCB layout, and a MATLAB/Simulink model of the control loop.

## Key Specifications

| Parameter | Value |
|---|---|
| Input Voltage (Vin) | 5 V |
| Output Voltage (Vout) | 12 V |
| Switching Frequency (fs) | 100 kHz |
| Target Load Current (Iout) | 1 A – 1.5 A (peak 2 A) |
| Control Scheme | Closed-loop PI control with dynamic PWM duty cycle generation |

## Design Approach

- The converter operates at 100 kHz switching frequency, chosen to [balance inductor/capacitor size against switching losses — replace with your actual reasoning].
- Inductor and output capacitor values were selected to keep output voltage ripple under [X]% and ensure continuous conduction mode at the target load range — fill in your actual values.
- The PI controller gains (Kp = [value], Ki = [value]) were tuned by [method used] to regulate output voltage against load transients.
- PWM duty cycle is generated dynamically based on the PI controller's error signal between reference (12V) and sensed output voltage.

## Repository Structure

- `DC-DC Boost converter/` — KiCad schematic (`.kicad_sch`), PCB layout (`.kicad_pcb`), and project files.
- `Simulation/` — MATLAB/Simulink closed-loop model (`.slx`) and simulation setup files.

## How to Run the Simulation

1. Open MATLAB and navigate to the `Simulation/` directory.
2. Open the `.slx` model in Simulink.
3. Run the simulation to observe the output voltage settling to 12V and the switching/PWM waveforms.

## Results

**Steady-state output voltage:** [X.X] V
**Settling time:** [X] ms
**Voltage ripple:** [X] mV / [X]%

## PCB

<img width="957" height="652" alt="image" src="https://github.com/user-attachments/assets/3d065906-f9c3-4757-a66a-0514c8531572" />
<img width="1037" height="587" alt="image" src="https://github.com/user-attachments/assets/5edd19ae-df37-4f0c-95d3-9f0bc8ec488c" />

Designed in KiCad.

## Reference & Original Work

Initial circuit topology was referred from a youtube guide for learning purpose. Building on that base, the closed-loop PI controller design, gain tuning, dynamic PWM duty cycle generation, and PCB schematic/layout in KiCad were done independently.

- [e.g. compare PI vs PID or peak-current-mode control]

