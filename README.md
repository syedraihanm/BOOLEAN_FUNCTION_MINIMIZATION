# EXP2:BOOLEAN FUNCTION MINIMIZATION

Name: Syed Mohamed Raihan

Reg No: 24900516


**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

![Screenshot 2024-11-25 102435](https://github.com/user-attachments/assets/97f72fe9-d795-4846-96eb-0631aa9bcfbf)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

module DE2(A, B, C, D, W, X, Y, Z, F1, F2);

input A, B, C, D,W,X,Y,Z;

wire x1, x2, x3, x4, x5, x6, x7, x8, x9, x10; output F1, F2;

assign x1=(~A) & (~B)&(~C)&(~D);

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



**RTL realization**


![Screenshot 2024-11-25 102435](https://github.com/user-attachments/assets/e07380e5-e6dd-487b-9608-45454ed0c2e3)


**Output:**


![Screenshot 2024-11-25 102937](https://github.com/user-attachments/assets/c6885172-0c4b-48f6-b5dc-4ff33c773189)




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

