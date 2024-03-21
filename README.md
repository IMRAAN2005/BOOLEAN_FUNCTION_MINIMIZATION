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
Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:SHAIK MAHAMMAD IMRAAN
 RegisterNumber:212223100053
module exp22(A,B,C,D,F1);
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


**RTL realization**

**Output:**

**RTL**
![RTL REAL](https://github.com/IMRAAN2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/149347407/1fa8ba8a-f945-4693-825e-74b97ff5fa02)
![TRUTH](https://github.com/IMRAAN2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/149347407/129009fd-0bc1-4125-b8ad-a54d8a863de1)


**Timing Diagram**
![OUTPUT](https://github.com/IMRAAN2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/149347407/808c49b0-32cd-483b-ad34-f61ab242306a)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

