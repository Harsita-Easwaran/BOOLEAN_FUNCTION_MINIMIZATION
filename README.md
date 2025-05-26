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

Developed by: Harsita Easwaran  RegisterNumber: 212224220036
'''
module BooleanFunction(a,b,c,d,f1); 
input a,b,c,d; 
output f1; 
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c)); 
endmodule

module BooleanFunction2(w,x,y,z,f2); 
input w,x,y,z; 
output f2; 
assign f2=((~y & z)|( w & y )|(x & y)); 
endmodule
'''
*/


**RTL realization**

**Output:**
![Screenshot 2025-05-26 205053](https://github.com/user-attachments/assets/17ef2d36-426b-49cf-85c6-dcd112fe21bb)
![Screenshot 2025-05-26 211137](https://github.com/user-attachments/assets/8b4b5819-6689-45d4-81d0-6372886eb712)


**Timing Diagram**
![Screenshot 2025-05-26 210225](https://github.com/user-attachments/assets/a2454b44-6d88-48c1-8d78-e88ec936acc6)
![Screenshot 2025-05-26 211305](https://github.com/user-attachments/assets/e7940c31-a577-47b6-bd6a-521b836fc6a6)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

