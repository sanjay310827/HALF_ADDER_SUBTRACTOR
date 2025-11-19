# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: SANJAY A
RegisterNumber: 25016505

```
Half-adder:

module hs (a,b,sum,carry);
input (a,b);
output (sum,carry);
xor gl(sum,a,b);
assign carry = a&b;
endmodule

Half-subtractor:

module hs (a,b, diff, borrow);
input (a,b);
output (diff, borrow);
xor gl(diff, a,b);
assign borrow = ~a&b;
endmodule
```

**RTL Schematic**

***Half-adder***
<img width="1912" height="1017" alt="ha" src="https://github.com/user-attachments/assets/6a9b0a52-2f4c-4de8-b184-7f69d3e80754" />

***Half-subtractor***
<img width="1919" height="1029" alt="image" src="https://github.com/user-attachments/assets/bf717d10-f11a-4039-90c6-2a625b19b8b1" />


**Output/TIMING Waveform**

***Half-adder***
<img width="1913" height="1022" alt="ha output" src="https://github.com/user-attachments/assets/ec648708-dd78-4fef-95ba-c345e2d35258" />


***Half-subtractor***
<img width="1920" height="1031" alt="image" src="https://github.com/user-attachments/assets/fc55cbb1-d745-47cb-9ad5-ca36e570d4e5" />


**Result:**
Thus the Implementation-of-Half-Adder-and-Half Subtractor-circuit was executed successfully.

