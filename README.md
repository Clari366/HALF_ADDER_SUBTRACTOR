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

half adder


![WhatsApp Image 2024-12-09 at 6 42 30 PM](https://github.com/user-attachments/assets/a8f92288-ac1e-4fad-89bd-f3376acbf9fd)

half subtracter


![WhatsApp Image 2024-12-09 at 6 42 58 PM](https://github.com/user-attachments/assets/65774ed0-c54e-4fff-8afc-01b1ecbf5a33)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: clarissa k RegisterNumber:24009830
```
module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule

```



```
module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule
```

**RTL Schematic**

half adder
![Screenshot 2024-11-05 081232](https://github.com/user-attachments/assets/8badc798-903d-4e53-97ad-2dd8a7004460)


half subtracter

![Screenshot 2024-11-05 082252](https://github.com/user-attachments/assets/bb266f04-e192-4a81-9502-bb95f6a118b1)


**Output/TIMING Waveform**

half adder

![Screenshot 2024-11-05 081603](https://github.com/user-attachments/assets/0e4a55ea-8449-4bab-8efd-281098ed2505)

half subtracter

![Screenshot 2024-11-05 082446](https://github.com/user-attachments/assets/7b1c2fd9-9ed2-4a8d-8215-f422b2a5c53a)


**Result:**
Thus the truth table of half adder and half subtractor circuit in Quartus II  using Verilog programming is verified.



