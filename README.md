# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: S.ANUSHARON 
RegisterNumber:  212222240010

For HALF ADDER:

module halfadder(a,b,s,c);
input a,b;
output s,c;
xor (s,a,b);
and (c,a,b);
endmodule

For FULL ADDER:

module fulladder(a,b,ci,s,co);
input a,b,ci;
output s,co;
wire d,e,f;
xor (d,a,b);
xor (s,d,ci);
and (e,ci,d);
and (f,a,b);
or (co,e,f);
endmodule

*/
Logic symbol & Truthtable



### Output:
### RTL

1.for Half adder

![Screenshot (229)](https://github.com/Anusharonselva/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119405600/2c099ba9-4741-4b73-8053-18cddb3befc2)

2.for Full adder


![Screenshot (230)](https://github.com/Anusharonselva/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119405600/d9399e59-eb83-4f3b-9e57-8b68a586de21)


### TIMING DIAGRAM

1.half adder


![Screenshot (231)](https://github.com/Anusharonselva/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119405600/cca41af5-f5c0-4ccd-8948-bd2c5845bfb2)

2.full adder

![Screenshot (232)](https://github.com/Anusharonselva/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119405600/503a2fb4-d6f0-4b76-9bd9-095877496322)

### TRUTH TABLE 

half adder

![Screenshot (233)](https://github.com/Anusharonselva/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119405600/da508ccd-49ba-4c55-bc33-218b7628e5ba)

full adder
![Screenshot (234)](https://github.com/Anusharonselva/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119405600/15add789-daf8-451d-8ad4-db5dc3ed2723)


### Result:
Thus half adder and full adder circuit is successfully designed and verified its truth table in Quartus using Verilog programming. About
