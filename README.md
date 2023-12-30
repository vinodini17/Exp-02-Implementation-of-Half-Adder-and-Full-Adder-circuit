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
### Program:
Half adder:

module de3hafeez(a,b,sum,carry);	                                                      input a,b;
output sum,carry; xor(sum,a,b);
and(carry,a,b);
endmodule

Full adder:

module de3_1(a,b,c,sum,carry);	                                                        input a,b,c;
output sum,carry; 
xor(sum,a,b,c);
assign carry=a&b|b&c|a&c; 
endmodule

Developed by: Vinodini R
RegisterNumber: 212223040244 

Logic symbol:
Half adder:
<img width="337" alt="image" src="https://github.com/vinodini17/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149347288/cdd2229f-f558-440c-9650-5199f83dd3d9">

Full adder:
<img width="376" alt="image" src="https://github.com/vinodini17/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149347288/41445239-57c3-4dd0-bc8c-19e23a334142">

Truthtable:
Half adder:
<img width="261" alt="image" src="https://github.com/vinodini17/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149347288/506357d9-ab23-44f7-9b96-2fd04aa55da5">

Full adder:
<img width="321" alt="image" src="https://github.com/vinodini17/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149347288/5254e68a-1d26-40fb-a9cb-0a6a52e2d69d">

RTL realization:

Half adder:
<img width="202" alt="image" src="https://github.com/vinodini17/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149347288/bc72fd4d-70cb-4e21-ab57-74ee5a775df9">

Full adder:
<img width="304" alt="image" src="https://github.com/vinodini17/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149347288/ef27cc78-786e-4aaa-a37d-d8167e326a96">

### TIMING DIAGRAM:

Half adder:
<img width="527" alt="image" src="https://github.com/vinodini17/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149347288/f7fa7508-1c91-4d62-8dfa-4733ad06a938">

Full adder:
<img width="960" alt="fulladder(w)" src="https://github.com/vinodini17/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149347288/64b4c4b2-752f-4603-b611-bf2ec7a46d2d">


### Result:
Thus the given logic functions are implemented and their operations are verified using verilog programming.

