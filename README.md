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

**HALF ADDER** :

![WhatsApp Image 2024-12-21 at 9 37 41 AM](https://github.com/user-attachments/assets/d169197f-3e66-4085-9ae9-4445bbad2ea3)

**HALF SUBTRACTER**

![WhatsApp Image 2024-12-21 at 9 36 46 AM](https://github.com/user-attachments/assets/de17c381-ee45-4cbc-b994-ce0de26b62b6)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: clarissa k RegisterNumber:24009830

**HALF ADDER**
```
module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule

```
**HALF SUBTRACTER**


```
module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule
```

**RTL Schematic**

**HALF ADDER**

![Screenshot 2024-11-05 081232](https://github.com/user-attachments/assets/8badc798-903d-4e53-97ad-2dd8a7004460)


**HALF SUBTRACTER**

![Screenshot 2024-11-05 082252](https://github.com/user-attachments/assets/bb266f04-e192-4a81-9502-bb95f6a118b1)


**Output/TIMING Waveform**

**HALF ADDERR**

![Screenshot 2024-11-05 081603](https://github.com/user-attachments/assets/0e4a55ea-8449-4bab-8efd-281098ed2505)

**HALF SUBTRACTTER**

![Screenshot 2024-11-05 082446](https://github.com/user-attachments/assets/7b1c2fd9-9ed2-4a8d-8215-f422b2a5c53a)


**Result:**
Thus the truth table of half adder and half subtractor circuit in Quartus II  using Verilog programming is verified.



