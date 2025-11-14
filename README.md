# EXPERIMENT 3A: Simulation of All Flip-Flops using Blocking Statement

## AIM
To design and simulate basic flip-flops (SR, D, JK, and T) using **blocking statements** in Verilog HDL, and verify their functionality through simulation in Vivado 2023.1.

## APPARATUS REQUIRED
- Vivado 2023.1
- Computer with HDL Simulator

## DESCRIPTION
Flip-flops are the basic memory elements in sequential circuits.  
In this experiment, different types of flip-flops (SR, D, JK, T) are modeled using **behavioral modeling** with **blocking assignment (`=`)** inside the `always` block.  
Blocking assignments execute sequentially in the given order, which makes it easier to describe simple synchronous circuits.

## PROCEDURE
1. Open **Vivado 2023.1**.  
2. Create a **New RTL Project** (e.g., `FlipFlop_Simulation`).  
3. Add Verilog source files for each flip-flop (SR, D, JK, T).  
4. Add a testbench file to verify all flip-flops.  
5. Run **Behavioral Simulation**.  
6. Observe waveforms of inputs and outputs for each flip-flop.  
7. Verify that outputs match the truth table.  
8. Save results and capture simulation screenshots.

---

## VERILOG CODE

### SR Flip-Flop (Blocking)
```verilog
module sr_ff (
    input wire S, R, clk,
    output reg Q
);
    always @(posedge clk) begin



endmodule
```
### SR Flip-Flop Test bench 
```verilog



```
#### SIMULATION OUTPUT

<img width="1920" height="1200" alt="Screenshot (50)" src="https://github.com/user-attachments/assets/c5da46ee-2934-4748-b00d-12dc8a34786f" />

---

### JK Flip-Flop (Blocking)
```verilog
module jk_ff (
    input wire J, K, clk,
    output reg Q
);
    always @(posedge clk) begin



endmodule
```
### JK Flip-Flop Test bench 
```verilog



```
#### SIMULATION OUTPUT


<img width="1920" height="1200" alt="Screenshot (51)" src="https://github.com/user-attachments/assets/5d73d470-8533-4c23-a91a-7e98346b95bf" />

---
### D Flip-Flop (Blocking)
```verilog
module d_ff (
    input wire d,clk,
    output reg Q
);
    always @(posedge clk) begin



endmodule
```
### D Flip-Flop Test bench 
```verilog



```

#### SIMULATION OUTPUT

<img width="1920" height="1200" alt="Screenshot (52)" src="https://github.com/user-attachments/assets/e6089e89-8542-4e9d-a7e6-53244d86eb7c" />

---
### T Flip-Flop (Blocking)
```verilog
module d_ff (
    input wire d,clk,
    output reg Q
);
    always @(posedge clk) begin



endmodule
```
### T Flip-Flop Test bench 
```verilog



```

#### SIMULATION OUTPUT

<img width="1285" height="620" alt="Screenshot 2025-09-22 111353" src="https://github.com/user-attachments/assets/80479ce8-dafe-47f5-a28d-6496c76e6acb" />


---

### RESULT

All flip-flops (SR, D, JK, T) were successfully simulated using blocking statements in Verilog HDL.
The outputs matched the expected truth table values, demonstrating correct sequential behavior.
