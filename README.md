# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.


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
module EXPERIMENT2(A,B,C,D,F1);

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

![image](https://github.com/user-attachments/assets/28312a06-5594-4fb1-8769-89c0abb8b6fc)



**Output:**


![436893172-0c245dab-2bdc-430c-bc75-2806b2c9a0c2](https://github.com/user-attachments/assets/a8a0682d-8e0d-488f-a4c9-151a699b3640)

**Timing Diagram**
![image](https://github.com/user-attachments/assets/4ef7c18c-d820-419b-9903-f2f740ee818b)





**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

