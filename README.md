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

Developed by: UDHAYDHARSHAN S
RegisterNumber: 212225230286
*/
```
module deexp2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)| (~a&b&d)| (a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
```
**RTL realization**
<img width="823" height="531" alt="image" src="https://github.com/user-attachments/assets/bb269ba7-2050-476f-86b6-3c969e8f9e61" />

**Output:**

**RTL**
<img width="1365" height="594" alt="image" src="https://github.com/user-attachments/assets/0b9ce858-64aa-4a71-8e34-43ad88bf6a7a" />


**Timing Diagram**
<img width="938" height="402" alt="image" src="https://github.com/user-attachments/assets/1d2b8fb0-0589-46c3-8748-18bd5ba921ed" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

