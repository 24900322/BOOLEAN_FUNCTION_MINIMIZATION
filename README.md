# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


Developed by:VIJAY M


RegisterNumber:24900322


**Program:**
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);

input A,B,C,D,W,X,Y,Z;

wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;

output F1,F2;

assign x1=(~A)&(~B)&(~C)&(~D);

assign x2=(A)&(~C)&(~D);

assign x3=(~B)&(C)&(~D);

assign x4=(~A)&(B)&(C)&(D);

assign x5=(B)&(~C)&(D);

assign x6=(X)&(~Y)&(Z);

assign x7=(~X)&(~Y)&(Z);

assign x8=(~W)&(X)&(Y);

assign x9=(W)&(~X)&(Y);

assign x10=(W)&(X)&(Y);

assign F1=x1|x2|x3|x4|x5;

assign F2=x6|x7|x8|x9|x10;

endmodule

**RTL realization**
![2024-09-24 090157](https://github.com/user-attachments/assets/d2744dd1-c428-4ec7-9276-a7a946de3701)


**Logic Symbol & Truthtable**
![2024-09-24 090236](https://github.com/user-attachments/assets/4a031cba-0300-40f4-ba72-e721ac636404)
![2024-09-24 090310](https://github.com/user-attachments/assets/2f18ec09-f41f-4ceb-92e5-74be317a1239)

**Output:**
![2024-09-24 090107](https://github.com/user-attachments/assets/7b26fcc0-4496-4b9c-b194-7cb6e141fcd7)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

