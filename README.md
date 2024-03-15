# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module ex2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);

assign F1=x1|x2|x3|x4|x5;
endmodule
```
Developed by: RAMKUMAR.S
RegisterNumber:212223220085


**RTL realization**
![image](https://github.com/Ramkumar1814/BOOLEAN_FUNCTION_MINIMIZATION/assets/151391179/9aa35bed-9354-461b-82fd-f5fdb4561c80)


**Output:**
![image](https://github.com/Ramkumar1814/BOOLEAN_FUNCTION_MINIMIZATION/assets/151391179/fefd2c41-6ada-4f98-ae0b-d8f8a36bbfec)


**Timing Diagram**
![image](https://github.com/Ramkumar1814/BOOLEAN_FUNCTION_MINIMIZATION/assets/151391179/b3fc3886-0fc5-4178-9e0a-4868d9c5f49f)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

