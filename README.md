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

Developed by: RegisterNumber:*/

module de2(a,b,c,d,w,x,y,z,f1,f2);

input a,b,c,d,w,x,y,z;

output f1,f2;

assign f1 = ~b&~d | a&b&~c | ~a&b&d;

assign f2 = ~y&z | x&y | w&y;

endmodule


**RTL realization**
<img width="639" height="490" alt="Screenshot 2026-05-21 133346" src="https://github.com/user-attachments/assets/41ff41da-2784-4c0e-bb90-7fe4e3826dd7" />


**Output:**

**RTL**
<img width="885" height="553" alt="Screenshot 2026-05-21 133722" src="https://github.com/user-attachments/assets/8d9741d4-adb8-49e7-bb3f-381ca5bd13fe" />


**Timing**

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

