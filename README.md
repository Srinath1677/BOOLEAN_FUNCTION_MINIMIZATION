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

Developed by: Srinath YG
RegisterNumber:212224230274

```verilog
module exp_2(A,B,C,D,F1);

input A,B,C,D;
output F1;

wire x1,x2,x3,x4,x5;

assign x1 = (~A) & (~B) & (~C) & (~D);
assign x2 = (A) & (~C) & (~D);
assign x3 = (~B) & (C) & (~D);
assign x4 = (~A) & (B) & (C) & (D);
assign x5 = (B) & (~C) & (D);

assign F1 = x1 | x2 | x3 | x4 | x5;

endmodule
```

**RTL realization**


![c90e6d22-7f9d-46a1-8770-2d86891860f2](https://github.com/user-attachments/assets/b1ea7bf2-03c1-4557-8091-d75db3cf4c7d)


**Output:**


![436893172-0c245dab-2bdc-430c-bc75-2806b2c9a0c2](https://github.com/user-attachments/assets/a8a0682d-8e0d-488f-a4c9-151a699b3640)

**RTL**
**Timing Diagram**

![fc9ff82c-6504-4a10-b125-dda35a9364ee](https://github.com/user-attachments/assets/34036003-5790-4699-a9a0-967d1cca35a4)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

