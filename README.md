
# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime

### Theory
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

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: SOWMYA V
RegisterNumber:  212222110045
1. HALF ADDER
module adder (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule

2. FULL ADDER
module fulladder(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum= a^b^cin;
assign carry = (a&b)|((a^b)&cin);
endmodule
```
## RTL DIAGRAM:
![image](https://github.com/SowmyaVisvanathan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119475775/0ba1d785-8c59-4d60-bcad-1f64610011eb)
![image](https://github.com/SowmyaVisvanathan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119475775/1fdf97dc-f3a4-43c6-b466-8a60aed7da1f)

### TRUTH TABLE:
1.HALF ADDER
![image](https://github.com/SowmyaVisvanathan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119475775/1c72ab50-b74f-4fde-ad74-56cdb5e993aa)

2.FULL ADDER
![image](https://github.com/SowmyaVisvanathan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119475775/c7c9242a-1830-4c56-9ac0-69988a12f81b)

### OUTPUT:
1.HALF ADDER
![image](https://github.com/SowmyaVisvanathan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119475775/71870c21-dcf8-421c-a0b8-6b42e7dc0e16)

2.FULL ADDER
![image](https://github.com/SowmyaVisvanathan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119475775/c5cb8d2b-463f-47c8-95b5-a93a5e0ed599)

### Result:
Thus the implementation of half adder and full adder circuit are stuided and the truth table for different logic gates are verified
