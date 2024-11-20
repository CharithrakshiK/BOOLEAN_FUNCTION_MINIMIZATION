# EXP2:BOOLEAN_FUNCTION_MINIMIZATION

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

module bool(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output f1,f2;
assign x1=(~a)&(~b)&(~c)&(~d);
assign x2=(a)&(~c)&(~d);
assign x3=(~b)&(c)&(~d);
assign x4=(~a)&(b)&(c)&(d);
assign x5=(b)&(~c)&(d);
assign x6=(x)&(~y)&(z);
assign x7=(~x)&(~y)&(z);
assign x8=(~w)&(x)&(y);
assign x9=(w)&(~x)&(y);
assign x10=(w)&(x)&(y);
assign f1=x1|x2|x3|x4|x5;
assign f2=x6|x7|x8|x9|x10;
endmodule 



Developed by: Charithrakshi K RegisterNumber: 24900651*/


**RTL realization**

![Screenshot 2024-11-20 203922](https://github.com/user-attachments/assets/90ed367e-693e-41ed-9448-575cbfad3a67)


**Output:**

![Screenshot 2024-11-20 205847](https://github.com/user-attachments/assets/864653c8-5517-4e46-990c-74dc87d67c2d)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

