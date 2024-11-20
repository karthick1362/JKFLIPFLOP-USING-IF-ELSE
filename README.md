# JKFLIPFLOP-USING-IF-ELSE

AIM:

To implement Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

SOFTWARE REQUIRED: 

Quartus prime

THEORY

JK Flip-Flop

JK flip-flop is the modified version of SR flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of JK flip-flop is shown in the following figure.

![image](https://github.com/user-attachments/assets/e6385ff4-e84e-44cd-942c-b876f75e5987)

This circuit has two inputs J & K and two outputs Qtt & Qtt’. The operation of JK flip-flop is similar to SR flip-flop. Here, we considered the inputs of SR flip-flop as S = J Qtt’ and R = KQtt in order to utilize the modified SR flip-flop for 4 combinations of inputs. The following table shows the state table of JK flip-flop.

![image](https://github.com/user-attachments/assets/a87c771f-55d2-48d4-b410-bf138d16562a)

Here, Qtt & Qt+1t+1 are present state & next state respectively. So, JK flip-flop can be used for one of these four functions such as Hold, Reset, Set & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of JK flip-flop. Present Inputs Present State Next State

![image](https://github.com/user-attachments/assets/08b499b2-8283-438e-9b02-0260c662621f)

By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. Three variable K-Map for next state, Qt+1t+1 is shown in the following figure.

![image](https://github.com/user-attachments/assets/5d65f332-e7a1-4894-ac3f-e30b7caa9821)

The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=JQ(t)′+K′Q(t)Q(t+1)=JQ(t)′+K′Q(t)

**Procedure**

step-1 Go to quartus software.

step-2 Set new environment.

step-3 Type the code to implement SR flipflop using verilog and validating their functionality using their functional tables.

step-4 Run the program.

step-5 Give inputs in the waveform table .

step-6 Run the program.

**PROGRAM**
/* Program for flipflops and verify its truth table in quartus using Verilog programming

module JK_FF(q,qb,j,k,clock);

input j,k,clock;

output reg q;

output qb;

always @(posedge(clock))

begin q <= (j&(~q))+ ((~k)&q);

end

assign qb = (~q);

 endmodule
 
 Developed by: **KARTHICK R**
RegisterNumber:**212223053002**

**RTL LOGIC FOR FLIPFLOPS** 

![image](https://github.com/user-attachments/assets/3c092ec6-8c5b-4d2e-bd00-6f15c73021fe)

**TIMING DIGRAMS FOR FLIP FLOPS**

![image](https://github.com/user-attachments/assets/8acbe071-b2c7-4051-9e00-284989c4169c)

**RESULT**

Thus implement JK flipflop using verilog and validating their functionality using their
functional tables has been successfully compeleted









