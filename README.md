### Name: VANA BHARATH.D
### Roll No: 23000857
# Experiment 03: Implementation of Half Adder and Full Adder circuit
# AIM
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.
# Equipments Required:
Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime
# Theory
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

# Procedure

Connect the supply (+5V) to the circuit

Switch ON the main switch

If the output is 1, then the led glows.






# Program:
### Half adder
module HalfAdder(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum=a^b;

assign carry=a&b;

endmodule

### Full adder
module Fulladder(a,b,c,sum,carry);

input a,b,c;

output sum,carry;

assign sum=((a^b)^c);

assign carry=((a&b) | (b&c) | (c&a));

endmodule

# RTL realization
### Half adder
![Exp 03 RTL realisation](https://github.com/amal-2006/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/148410730/b30a988e-85cf-4d33-85c1-38826dea1b45)

### Full adder
![Exp 3 Full adder RTL realization](https://github.com/amal-2006/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/148410730/e75af70a-0cab-4024-9c7d-8cb6d3cfd843)


# Truth Table
### Half adder
![Exp 3 half adder  truth table](https://github.com/amal-2006/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/148410730/895b059f-09b6-43a7-b003-b8dc05f6ee88)

### Full adder
![Exp 3 full adder truth table](https://github.com/amal-2006/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/148410730/ea912e57-4abb-4002-b981-63c66c397783)

# Timing Diagram
### Half adder
![Exp 03 Timing Diagram](https://github.com/amal-2006/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/148410730/6637ebc6-60c4-463a-b1ac-4bca2edff20a)

### Full adder
![Exp 3 Full adder Timing Diagram](https://github.com/amal-2006/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/148410730/e04818be-43ff-440a-981a-0dcef8eda3a7)

# Result
Hence, the output is verified successfully.
