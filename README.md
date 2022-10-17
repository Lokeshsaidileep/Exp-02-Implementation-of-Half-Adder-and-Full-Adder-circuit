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
Developed by:S.LOKESH SAI DILEEP
RegisterNumber:212221230111 
*/
HALF ADDER
/*
module Adder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule
/*
FULL ADDER
/*
module FullAdder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule
/*
### Output:
### RTL
![image](https://user-images.githubusercontent.com/94883079/196163955-68a42318-b632-4f30-9a0b-29f4b903f565.png)

### TIMING DIAGRAM
![image](https://user-images.githubusercontent.com/94883079/196163992-6b1028e1-6d1d-4841-b1bb-0494ac8a0285.png)

### TRUTH TABLE 
![image](https://user-images.githubusercontent.com/94883079/196164048-be0fef67-0ab2-447c-989a-1df59e9696b9.png)

FULL ADDER
### RTL
![image](https://user-images.githubusercontent.com/94883079/196164204-bd8a14be-e00c-4c0f-b5d9-b8bdc08c6752.png)

### TIMING DIAGRAM
![image](https://user-images.githubusercontent.com/94883079/196164255-e95948cc-b018-47e2-a4ec-af5208a487a1.png)

### TRUTH TABLE
![image](https://user-images.githubusercontent.com/94883079/196164351-02e8f5a3-7e7e-48a1-8a15-c981aec883ee.png)

### Result:
Thus, a half adder and full adder circuit is designed to verify its truth table in Quartus using Verilog programming.


