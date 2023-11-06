### EXP-03-IMPLEMENTATION OF HALF ADDER AND FULL ADDER CIRCUIT
## AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

## EQUIPMENTS REQUIRED:
Hardware – PCs, Cyclone II , USB flasher Software – Quartus prime

## THEORY:
Adders are digital circuits that carry out addition of numbers.

## Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

## Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

![image](https://github.com/ChandrasekarS22008273/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119643845/07fcae06-a77f-4329-8610-0eee0d3441da)


## Figure -01 HALF ADDER
![image](https://github.com/ChandrasekarS22008273/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119643845/9b98f3ba-2391-42f2-8f1e-859f9dba225a)


## Figure -02 FULL ADDER
## PROCEDURE:
Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
## PROGRAM:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Chandrasekar
RegisterNumber: 212222230025

1. Program to design a half adder:

module ex3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule 
```
```
2. Program to design a full adder:

module ex31(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^cin;
assign carry=(a&b)|((a^b)&cin);
endmodule
```
## TRUTH TABLE:
## HALF ADDER
![image](https://github.com/ChandrasekarS22008273/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119643845/ba081a4c-a541-4a4f-920b-0845a6dacdfc)


## FULL ADDER
![image](https://github.com/ChandrasekarS22008273/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119643845/754fc98c-98da-4a21-a400-449e3acbdeb3)


## RTL REALIZATION:
## HALF ADDER
![image](https://github.com/ChandrasekarS22008273/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119643845/cee27315-48f9-4e40-a5fc-56fa0e64f3e2)


## FULL ADDER
![image](https://github.com/ChandrasekarS22008273/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119643845/e9d0cc82-778d-423a-b249-43d640ee034a)


## OUTPUT WAVEFORM:
## HALF ADDER
![image](https://github.com/ChandrasekarS22008273/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119643845/2531db7c-31d7-4bed-9cea-61b608ca73e3)


## FULL ADDER
![image](https://github.com/ChandrasekarS22008273/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119643845/90e35198-d3f2-4bc4-a6ff-d749174ee62e)


## RESULT:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.
