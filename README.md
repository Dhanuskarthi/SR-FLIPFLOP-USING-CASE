# SR-FLIPFLOP-USING-CASE

**AIM:**

To implement  SR flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

SR Flip-Flop SR flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, SR latch operates with enable signal. The circuit diagram of SR flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/SR-FLIPFLOP-USING-CASE/assets/154305477/0f710028-ad52-4d3e-9276-8714cf023a25)

 
This circuit has two inputs S & R and two outputs Qtt & Qtt’. The operation of SR flipflop is similar to SR Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of SR flip-flop.

![image](https://github.com/naavaneetha/SR-FLIPFLOP-USING-CASE/assets/154305477/dabfc4f4-87e3-4cbc-9472-f89ee1b5ed30)

 
Here, Qtt & Qt+1t+1 are present state & next state respectively. So, SR flip-flop can be used for one of these three functions such as Hold, Reset & Set based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of SR flip-flop. Present Inputs Present State Next State

![image](https://github.com/naavaneetha/SR-FLIPFLOP-USING-CASE/assets/154305477/dd90d16c-aec5-4290-a586-e2346b1e9eb5)

 
By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. The three variable K-Map for next state, Qt+1t+1 is shown in the following figure.

![image](https://github.com/naavaneetha/SR-FLIPFLOP-USING-CASE/assets/154305477/473efad6-d70b-4ca7-aeb7-898bbfca319f)

 
The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=S+R′Q(t)Q(t+1)=S+R′Q(t)

**Procedure**

/* write all the steps invloved */
*1*.Open quartus II and create New project wizard.
*2*. Write the program in Verilog HDL file and run the program.
*3*. Download the RTL viewer.
*4*. Now open university program VWF and download waveform after the execution.

**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming.

module EXP_6(S,R,clk,Q,Qbar); input S,R,clk; output reg Q; output reg Qbar; initial Q=0; initial Qbar=1; always @(posedge clk) begin Q=S|((~R)&Q); Qbar=~Q; end endmodule

Developed by: RegisterNumber:
*/24005701

**RTL LOGIC FOR FLIPFLOPS**

![387143499-11d45f3c-13f2-4d3b-b998-e3ccbd2017cb](https://github.com/user-attachments/assets/15b6bd4a-e941-4fac-84dc-82e080109f6c)

**TIMING DIGRAMS FOR FLIP FLOPS**

![387143375-8b30be26-232f-4adb-acc6-6277abd53319](https://github.com/user-attachments/assets/2b5a7a71-3989-46da-85f4-59d3e80818a3)

**RESULTS**
Thus the Flip flop designed and the truth tables is verified using Quartus software.
