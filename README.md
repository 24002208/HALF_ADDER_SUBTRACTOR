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

**Truthtable**

![WhatsApp Image 2024-12-21 at 09 37 41_18d96a21](https://github.com/user-attachments/assets/35b4182d-e199-4d26-9688-7629a12339d1)

![WhatsApp Image 2024-12-21 at 09 36 46_b850d9bf](https://github.com/user-attachments/assets/ad3371e7-f5fa-4623-b46e-33c01cee53e3)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

 i)HALF ADDER
 module ha(a,b,sum,carry);
 
 input a,b;
 
 output sum,carry;
 
 assign sum= (a ^ b);
 
 assign carry= ( a & b);
 
 endmodule
 
 ii)HALF SUBTRACTOR
 module hs(a,b,difference,borrow);
 
 input a,b;
 
 output difference,borrow;
 
 assign difference= (a ^ b);
 
 assign borrow= ( ~a & b);
 
 endmodule
 

Developed by: S.Dhamini

RegisterNumber:24002208

**RTL Schematic**

![WhatsApp Image 2024-12-22 at 22 45 10_e01f6be7](https://github.com/user-attachments/assets/03284168-629a-4a5a-a002-6c42331d1c3c)

![WhatsApp Image 2024-12-22 at 22 39 41_2334b6c5](https://github.com/user-attachments/assets/ffc8c88a-1802-43e4-b2ca-e0a49b584f83)

**Output/TIMING Waveform**

![WhatsApp Image 2024-12-22 at 23 46 45_e5148826](https://github.com/user-attachments/assets/2934975b-5a08-43f7-a81b-505afaebd167)

![WhatsApp Image 2024-12-22 at 23 40 52_f5f0c2fa](https://github.com/user-attachments/assets/dae9d661-7d76-4076-952f-b100454db550)

**Result:**

A half adder and half subtractor circuit is verified its truth table in Quartus using Verilog programming.


