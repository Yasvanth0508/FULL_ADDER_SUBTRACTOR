# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

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

**Procedure**

Write the detailed procedure here

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
**Program:**
```

module exp4(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=( (a ^ b)^c);
assign carry= ( (a & b)| ( cin &(a ^ b ));
endmodule


module exp4(a,b,difference,borrow);
input a,b,bin;
output difference,borrow;
assign difference= ( (a ^ b)^bin);
assign borrow= ( ( ~a & b)| ( bin & (~(a ^ b )));
endmodule

Developed by:Yasvanth RD
RegisterNumber:24900517

```

**RTL Schematic**

![WhatsApp Image 2024-12-04 at 14 12 36_0c82ccf1](https://github.com/user-attachments/assets/c0a1c90c-e8d8-42b5-9e9e-58f27e437a93)
![WhatsApp Image 2024-12-04 at 14 12 36_0c01e239](https://github.com/user-attachments/assets/b5d2d184-efaa-4cc1-972b-10fa0cbb4c17)

**Output Timing Waveform**

![WhatsApp Image 2024-12-04 at 14 12 36_4c4a3740](https://github.com/user-attachments/assets/a50708e5-5efb-4312-9a09-f223262edbbd)
![WhatsApp Image 2024-12-04 at 14 12 35_142a4147](https://github.com/user-attachments/assets/629f77c1-73ca-4709-b361-43cbeb6893ea)


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



