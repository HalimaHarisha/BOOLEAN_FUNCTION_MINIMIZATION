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

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: HALIMA HARISHA A

RegisterNumber:24901005

```
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule
```
**Truth Table**

![Screenshot 2024-12-06 213338](https://github.com/user-attachments/assets/1d67ce18-c379-42b9-a0a3-6bcfd25fd258)

![Screenshot 2024-12-06 213346](https://github.com/user-attachments/assets/a3f63749-6bfb-4d75-8652-d58c69803a72)


**Output:**

**RTL**

![Screenshot 2024-12-06 213440](https://github.com/user-attachments/assets/3fce23c4-912a-44ab-b707-36cdd706b109)

**Timing Diagram**

**RTL realization**

![Screenshot 2024-12-06 213450](https://github.com/user-attachments/assets/bb6437f1-a6d8-4ea6-be06-4fe521fe9ecf)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

