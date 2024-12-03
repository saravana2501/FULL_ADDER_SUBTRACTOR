**EXP4:FULL ADDER AND SUBTRACTOR**

NMAE: SARAVANA KUMAR

REF NO :24900200


**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**


FULL ADDER

![image](https://github.com/user-attachments/assets/f498c445-fd3a-4e79-9e8a-3aabef86d2a4)


FULL SUBRACTOR

![image](https://github.com/user-attachments/assets/26d770f8-64ef-4266-b758-8090fa9b32d4)


**Procedure**

Write the detailed procedure here

**Program:**

 Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:

 FULL ADDER

module fulladder(a,b,cin,sum,carry);

input a,b,cin;

output sum,carry;

assign sum=( (a ^ b)^cin);

assign carry= ( (a & b)| ( cin &(a ^ b )));

endmodule


 FULL SUBRACTOR

module fullsubractor(a,b,bin,difference,borrow);

input a,b,bin;

output difference,borrow;

assign difference= ( (a ^ b)^bin);

assign borrow= ( ( a & b)| ( bin & ((a ^ b ))));

endmodule
 

**RTL Schematic**

FULL ADDER

![full adder logic gate screenshot](https://github.com/user-attachments/assets/185d5335-bbd7-4078-b1eb-53173a2ecf28)



FULL SUBRACTOR


![full subtractor logic gate screenshot](https://github.com/user-attachments/assets/e62e8038-7a2e-4bb0-8c5a-ebee2e2b6c7e)


**Output Timing Waveform**

FULL ADDER

![full adder waveform screenshot](https://github.com/user-attachments/assets/b63e98de-4216-44ec-9102-82080407e08e)




FULL SUBRACTOR


![full subtractor waveform screenshot](https://github.com/user-attachments/assets/2a6a5327-cd60-40a5-8e0b-3a85be8bf88b)



**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



