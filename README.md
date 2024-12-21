# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a Half Adder and Half Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Adder Truth Table**

![half adder](https://github.com/user-attachments/assets/93b62dbb-1f2e-4bde-9d62-761303058465)

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Half Subtractor Truth Table**

![half subtractor](https://github.com/user-attachments/assets/d131d52d-8ea2-4ae8-95d6-a2d5ad12f359)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and Half Subtactor circuit and verify its truth table in quartus using Verilog programming.

Developed by: P Sirisha RegisterNumber: 24002102

Half Adder
```
module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=(a^b);
assign carry=(a&b);
endmodule
```

Half Subtractor
```
module hs(a,b,diff,borr);
input a,b;
output diff,borr;
assign diff=(a^b);
assign borr=(~a&b);
endmodule
```

**RTL Schematic**

Half Adder
![ex 3a](https://github.com/user-attachments/assets/1c78a009-ea42-4b45-b53a-7ec3be56cd0f)

Half Subtractor
![ex 3b](https://github.com/user-attachments/assets/f0e41a11-1be6-4f9d-9742-cb9579cb7434)

**Output**

Half Adder

![ex 3a wave](https://github.com/user-attachments/assets/568949d5-9b0b-483b-88d2-4e92689bbf9d)

Half Subtractor

![ex 3b wave](https://github.com/user-attachments/assets/225fe057-fa9d-49a0-b8f7-3cbf5771517e)

**Result:**
 Half Adder and Half Subtractor circuit and  its truth table in Quartus using Verilog programming is verified.
