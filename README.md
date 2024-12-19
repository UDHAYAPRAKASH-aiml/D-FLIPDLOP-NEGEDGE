# D-FLIPDLOP-NEGEDGE

**AIM:**

To implement  D flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**D Flip-Flop**

D flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, D latch operates with enable signal. That means, the output of D flip-flop is insensitive to the changes in the input, D except for active transition of the clock signal. The circuit diagram of D flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/48c81fe8-bc3f-40e7-95e2-519fc155ad51)

This circuit has single input D and two outputs Qtt & Qtt’. The operation of D flip-flop is similar to D Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of D flip-flop.

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/e5f3fda7-68ec-4a3a-a0a4-cf6f9cc4ab55)

Therefore, D flip-flop always Hold the information, which is available on data input, D of earlier positive transition of clock signal. From the above state table, we can directly write the next state equation as Qt+1t+1 = D

![image](https://github.com/naavaneetha/D-FLIPDLOP-NEGEDGE/assets/154305477/8592c0d8-2917-4142-91b9-d6c30dd891d2)

Next state of D flip-flop is always equal to data input, D for every positive transition of the clock signal. Hence, D flip-flops can be used in registers, shift registers and some of the counters.
```
**Procedure**
/* write all the steps invloved */:
step 1: first go to qratus prime software
step2: create folder and type the program
step3:In the veriog you get RTL diagram
step4:And the waveform diagram
step 5:end the program 
```
```
**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming.
Developed by: Udhaya prakash v
RegisterNumber:24901131
module d_flipflop (
    input clk,    // Clock signal
    input reset,  // Active-high reset signal
    input d,      // Data input
    output reg q  // Output
);
    always @(posedge clk or posedge reset) begin
        if (reset) 
            q <= 1'b0; // Reset the output to 0
        else 
            q <= d;    // Capture the value of d on clock edge
    end
endmodule
*/
```
**RTL LOGIC FOR FLIPFLOPS**:

![de 8 o](https://github.com/user-attachments/assets/ec9d4eea-c8a2-4cdf-95c6-eb7df47d3791)


**TIMING DIGRAMS FOR FLIP FLOPS**
![de 8w](https://github.com/user-attachments/assets/7b434f61-a87f-4576-b16d-e86b819123a4)


**RESULTS**:
Thus the D-flip flop and truth table are verified
