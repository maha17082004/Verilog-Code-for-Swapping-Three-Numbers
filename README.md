# Verilog-Code-for-Swapping-Three-Numbers
## Aim
```
To design and simulate a Verilog HDL code for swapping the values of three numbers without using any temporary variables, and verify the correctness of the swapping operation through a testbench using the Vivado 2023.1 simulation environment.
```
## Apparatus Required
```
Vivado 2023.1 or equivalent Verilog simulation tool.
```
## Procedure
```
Launch Vivado 2023.1:

Open Vivado and create a new project.
Write the Verilog Code for Swapping:

Write the Verilog code that swaps the values of three numbers (a, b, and c) using basic arithmetic or bitwise operations without using temporary variables.
Create the Testbench:

Write a testbench to simulate the swapping operation. The testbench should initialize three numbers, trigger the swapping module, and check if the values are swapped correctly.
Add the Verilog Files:

Add the Verilog module and the testbench file to the Vivado project.
Run Simulation:

Run the behavioral simulation in Vivado to verify the swapping operation.
Observe the Waveforms:

Examine the waveform to confirm that the values of the three numbers are swapped as expected.
Save and Document Results:

Capture the waveform output and include the results in your report for verification.
```
## Verilog Code:
```
module swap_three_numbers ( a_in,b_in,c_in,a_out,b_out,c_out);
    input wire [7:0] a_in;
    input wire [7:0] b_in;
    input wire [7:0] c_in;
    output reg [7:0] a_out;
    output reg [7:0] b_out;
    output reg [7:0] c_out;
    always @(*) begin
        a_out = b_in; 
        b_out = c_in; 
        c_out = a_in; 
    end
endmodule
```
## OUTPUT
![WhatsApp Image 2024-10-17 at 17 41 26_aae0361a](https://github.com/user-attachments/assets/f2bc7b1a-a2f0-44a9-9dcf-22d5811963f5)
![WhatsApp Image 2024-10-17 at 17 41 42_f60b79a5](https://github.com/user-attachments/assets/e7275e78-ef43-415e-ad5c-ead3ff200f6e)
![WhatsApp Image 2024-10-17 at 17 41 56_4469fb58](https://github.com/user-attachments/assets/feb9b2ef-f01d-4fe4-9625-d65080898285)

## Conclusion
```
In this experiment, a Verilog HDL code for swapping three numbers was designed and successfully simulated. The testbench verified the swapping operation, showing that the values of three input numbers (a, b, and c) were swapped correctly without the use of temporary variables. This experiment demonstrated the effectiveness of Verilog in implementing logical operations and control mechanisms such as swapping values. The simulation results confirm the correct functionality of the design.
```
