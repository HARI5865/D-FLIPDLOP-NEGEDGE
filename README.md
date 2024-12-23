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

**Procedure**

/* write all the steps invloved */

**PROGRAM**<br>
module exp8(D,clk,Q,Qbar);<br>
input D,clk;<br>
output reg Q;<br>
output reg Qbar;<br>
initial Q=0;<br>
initial Qbar =1;<br>
always @ (posedge clk)<br>
begin<br>
Q=D;<br>
Qbar = ~D;<br>
end<br>
endmodule<br>

/* Program for flipflops and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:
*/

**RTL LOGIC FOR FLIPFLOPS**<br>
![390975348-976eccdb-30a3-4798-92fc-29aa1e3e170c](https://github.com/user-attachments/assets/9e3f60e3-ba53-4f27-b0dc-6cf49395eadf)



**TIMING DIGRAMS FOR FLIP FLOPS**<br>
![390975396-b7af813b-9678-433a-9963-25a6d371fe78](https://github.com/user-attachments/assets/e96935e4-28d8-47d4-8628-f80c8e32ff3e)



**RESULTS**<br>
To implement D flipflop using verilog and validating their functionality using their functional tables are verified.
