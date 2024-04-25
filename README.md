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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: VINCY JOVITHA V
Register Number: 212223230242
*/
```
module ex02(A,B,C,D,F1);
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

**Truth Table:**
![Screenshot 2024-04-25 142336](https://github.com/VincyJovitha01/BOOLEAN_FUNCTION_MINIMIZATION/assets/147121113/e83900d0-6bc3-4ce8-9dd9-d2fd234bc4d0)

**RTL realization**
![DE](https://github.com/VincyJovitha01/BOOLEAN_FUNCTION_MINIMIZATION/assets/147121113/a67ab28f-c09c-48b2-8370-918b1a7dceed)

**Output:**
**RTL**
**Timing Diagram**
![image](https://github.com/VincyJovitha01/BOOLEAN_FUNCTION_MINIMIZATION/assets/147121113/4e0c5754-ac73-4f68-8e37-9fb4aceffd73)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

