# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Salini .A RegisterNumber:*/ 212223220091
```
module ex2(A,B,C,D,F1);
input A, B, C, D;
output F1;
wire x1, x2, x3, x4, x5;
assign x1=(~A)&(~B)&(~C) & (~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```
**RTL REALIZATION**
![Screenshot 2024-03-20 220212](https://github.com/salinianbzhgan/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742862/d823a8fa-8bca-4b0b-b4bf-50d4a59bef67)
**TRUTH TABLE**
![Screenshot 2024-03-20 220253](https://github.com/salinianbzhgan/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742862/11609667-ab11-4538-a0bf-29f5101c9ce3)
**TIMING DIADRAM**

![Screenshot 2024-03-20 220317](https://github.com/salinianbzhgan/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742862/f230d363-40c9-4ef6-8faf-e5102a55f37b)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

