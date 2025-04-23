# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit
```
Developed by: MADHESH I
Reg No: 212224220055
```
**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)



**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)



**Truthtable**
![WhatsApp Image 2024-12-03 at 13 56 18_f1228d65](https://github.com/user-attachments/assets/326e7294-3fe0-4c26-aa22-207434d4e2a2)

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


**RTL Schematic**
HALF ADDER
![Screenshot 2024-12-03 132819](https://github.com/user-attachments/assets/3e33c7f4-7647-4daf-969e-433462b69399)
HALF SUBTRACTOR
![Screenshot 2024-12-03 133936](https://github.com/user-attachments/assets/90e73d87-3870-42a6-97ea-de3dc820ea91)
**Output/TIMING Waveform**
HALF ADDER
![Screenshot 2024-12-03 133409](https://github.com/user-attachments/assets/05abc62c-8448-416c-a86f-5a83c9885162)
HALF SUBTRACTOR
![WhatsApp Image 2024-12-03 at 13 59 02_b012424c](https://github.com/user-attachments/assets/063f6607-46dd-45e5-a224-d410bc801d12)


**Result:**
THe truthtable of half adder and Half subtractor in quartus 2 using verilog programming are studied,verified and executed successfully.
