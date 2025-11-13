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

**PROGRAM**
```
module EXP8DE(D,Clock,reset,Q,Qbar);
input D,Clock,reset;
output reg Q,Qbar;
always @(negedge Clock)
if(!reset)
	Q<=0;
else
	Q<=D;
endmodule
```

```
/* Program for flipflops and verify its truth table in quartus using Verilog programming. 
Developed by: RITHVIK S
RegisterNumber: 212223100045
*/
```

**RTL LOGIC FOR FLIPFLOPS**
<img width="737" height="332" alt="326327098-62373e4d-0689-4b80-842e-165057294500" src="https://github.com/user-attachments/assets/2033fe28-feeb-4a7d-be50-aeec3ac52920" />


**TIMING DIGRAMS FOR FLIP FLOPS**

<img width="1918" height="505" alt="326327117-4b72f1cc-faa4-4acf-88c3-8cc9ba3361fa" src="https://github.com/user-attachments/assets/39cbe356-b687-4fdb-8a54-824924739069" />

**RESULTS**
