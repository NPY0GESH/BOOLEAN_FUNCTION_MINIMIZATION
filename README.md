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
module exp2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/25004682
**RTL REALIZATION**
<img width="789" height="639" alt="image" src="https://github.com/user-attachments/assets/3b6008c9-3870-471f-b370-71e506760317" />


**RTL**
<img width="505" height="630" alt="image" src="https://github.com/user-attachments/assets/2e16391d-4daa-40c1-b931-ff361c87df44" />

**Timing Diagram**
<img width="814" height="208" alt="image" src="https://github.com/user-attachments/assets/5ffa26a9-c5e9-4556-a623-f38e2a82c3a8" />
**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

