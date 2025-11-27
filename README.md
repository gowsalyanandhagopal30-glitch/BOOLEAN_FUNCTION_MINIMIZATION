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
module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
```

**Boolean logic circuit**
![WhatsApp Image 2025-11-27 at 1 06 02 PM](https://github.com/user-attachments/assets/5af428d9-7a85-4304-83cd-d502c955c99a)

**RTL realization**
<img width="1920" height="1080" alt="Screenshot (56)" src="https://github.com/user-attachments/assets/fe61b26b-5431-4945-8fdc-8facb7f10f23" />

**Output:RTL**
<img width="1920" height="1080" alt="Screenshot (57)" src="https://github.com/user-attachments/assets/ba644426-5286-46d5-b3b8-46a24c8c599f" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

