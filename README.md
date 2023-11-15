# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

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
Connect the supply (+5V) to the circuit Switch ON the main switch If the output is 1, then the led glows.

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: BALASUDHAN P
RegisterNumber: 212222240017

1. Program to design a half adder:

module ex3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule 

2. Program to design a full adder:

module ex31(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^cin;
assign carry=(a&b)|((a^b)&cin);
endmodule

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: 
RegisterNumber:  
*/
Logic symbol & Truthtable
RTL realization

### TRUTH TABLE

HALF ADDER

![266758602-9b4a71eb-8d15-4ecd-b42f-38f3636c6e1b](https://github.com/BALASUDHAN18/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118807740/9fc6179e-8405-4424-b138-bf8e06ec2484)


FULL ADDER
![266758619-629eae2f-49e4-45c9-883a-42305ca95f2c](https://github.com/BALASUDHAN18/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118807740/36bfeec3-b0db-4bf6-b05d-ba0cdf405263)

### RTL

![266758666-d8ac11fc-a13f-4ca7-afb5-5010992a3a99](https://github.com/BALASUDHAN18/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118807740/f16f4328-5607-4d5a-97cf-fb6712ebd666)


### Output:
HALF ADDER

![266758710-5357d606-086d-4bc6-a757-2f6e15881137](https://github.com/BALASUDHAN18/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118807740/32ae58b8-1228-47d1-953a-4bab1a471ed3)

FULL ADDER

![266758724-41b25b21-d2ef-4ff0-b67d-dca564172dd8](https://github.com/BALASUDHAN18/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118807740/19a4fc92-08a9-4ead-8581-d095662be91a)

### Result:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.
