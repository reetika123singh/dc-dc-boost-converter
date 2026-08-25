# DC-DC Boost Converter Design & Simulation

An open-source DC-DC Boost Converter project featuring custom KiCad schematic and PCB layout, and a Simulink dynamic simulation model.

## Key Specifications
* **Input Voltage ($V_{in}$):** 5V
* **Output Voltage ($V_{out}$):** 12V
* **Switching Frequency ($f_s$):** 100 kHz
* **Target Load Current ($I_{out}$):** 1A to 1.5A (Peak value= 2A)

## Project Structure
* `DC-DC Boost converter/`: KiCad schematic (`.kicad_sch`), PCB layout (`.kicad_pcb`), and project files.
* `Simulation/`: MATLAB/Simulink models (`.slx`) and simulation setup files.

## How to Run Simulation
1. Open MATLAB and navigate to the `Simulation/` directory.
2. Open the `.slx` model file in Simulink.
3. Run the simulation to view voltage boost dynamics and switching waveforms.

## Credits
* Based on a YouTube tutorial guide.

