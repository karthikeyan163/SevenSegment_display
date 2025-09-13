Exp-No: 02 - Write and simulate seven segment display using Verilog HDL and verify with testbench
Aim:

  To design and simulate a Seven Segment using Verilog HDL and verify its functionality through a testbench using the Vivado 2023.1 simulation environment.
Apparatus Required:

  Vivado 2023.1

Procedure:


Launch Vivado Open Vivado 2023.1 by double-clicking the Vivado icon or searching for it in the Start menu.
Create a New Project Click on "Create Project" from the Vivado Quick Start window. In the New Project Wizard: Project Name: Enter a name for the project (e.g., Mux4_to_1). Project Location: Select the folder where the project will be saved. Click Next. Project Type: Select RTL Project, then click Next. Add Sources: Click on "Add Files" to add the Verilog files (e.g., mux4_to_1_gate.v, mux4_to_1_dataflow.v, etc.). Make sure to check the box "Copy sources into project" to avoid any external file dependencies. Click Next. Add Constraints: Skip this step by clicking Next (since no constraints are needed for simulation). Default Part Selection: You can choose a part based on the FPGA board you are using (if any). If no board is used, you can choose any part, for example, xc7a35ticsg324-1L (Artix-7). Click Next, then Finish.
Add Verilog Source Files In the "Sources" window, right-click on "Design Sources" and select Add Sources if you didn't add all files earlier. Add the Verilog files (mux4_to_1_gate.v, mux4_to_1_dataflow.v, etc.) and the testbench (mux4_to_1_tb.v).
Check Syntax Expand the "Flow Navigator" on the left side of the Vivado interface. Under "Synthesis", click "Run Synthesis". Vivado will check your design for syntax errors. If any errors or warnings appear, correct them in the respective Verilog files and re-run the synthesis.
Simulate the Design In the Flow Navigator, under "Simulation", click on "Run Simulation" → "Run Behavioral Simulation". Vivado will open the Simulations Window, and the waveform window will show the signals defined in the testbench.
View and Analyze Simulation Results 
Adjust Simulation Time To run a longer simulation or adjust timing, go to the Simulation Settings by clicking "Simulation" → "Simulation Settings". Under "Simulation", modify the Run Time (e.g., set to 1000ns).
Generate Simulation Report Once the simulation is complete, you can generate a simulation report by right-clicking on the simulation results window and selecting "Export Simulation Results". Save the report for reference in your lab records.
Save and Document Results Save your project by clicking File → Save Project. Take screenshots of the waveform window and include them in your lab report to document your results. You can include the timing diagram from the simulation window showing the correct functionality of the Seven Segment across different select inputs and data inputs.
Close the Simulation Once done, by going to Simulation → "Close Simulation

Input/Output Signal Diagram:

<img width="640" height="400" alt="image" src="https://github.com/user-attachments/assets/a2f6ea7e-4871-4a01-a021-fe8b632c5587" />

RTL Code:

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/365b612a-6a2d-4de7-b414-40b358bf68fe" />

TestBench:

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/e048efbd-af78-47de-b47a-f0fa7cf8523e" />

Output waveform:

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/b5101357-6f21-4c3b-b242-a1f48fd3d76b" />

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/e87a960c-e1f0-4112-a47c-d5eb31254857" />

Output waveform:

Conclusion:
The Seven-Segment Display was successfully designed and simulated using Verilog HDL in Vivado 2023.1. The testbench verified that the output matched the expected segment patterns for all inputs, confirming correct functionality.
