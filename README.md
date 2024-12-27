**FULL_ADDER_SUBTRACTOR**

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**EQUIPMENTS REQUIRED:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**FULL ADDER AND FULL SUBTRACTOR:**

**FULL ADDER:**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**FULL SUBTRACTOR:**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**TRUTH TABLE:**

FULL ADDER:

![image](https://github.com/user-attachments/assets/de47df46-b5b3-4715-b158-d56a4b83ea90)


FULL SUBTRACTOR:

![image](https://github.com/user-attachments/assets/025b7b50-c883-486e-a9d3-73983b67da89)


**PROCEDURE:**

1. Type the program in Quartus software.
2. Compile and run the program.
3. Generate the RTL schematic and save the logic diagram.
4. Create nodes for inputs and outputs to generate the timing diagram.
5. For different input combinations generate the timing diagram

**PROGRAM:**

)FULL ADDER

    module fa(a,b,cin,sum,carry);
    input a,b,cin;
    output sum,carry;
    assign sum=( (a ^ b)^cin);
    assign carry= ( (a & b)| ( cin &(a ^ b )));
    endmodule

ii)FULL SUBTRACTOR

    module fs(a,b,bin,difference,borrow);
    input a,b,bin;
    output difference,borrow;
    assign difference= ( (a ^ b)^bin);
    assign borrow= ( ( ~a & b)| ( bin & (~(a ^ b ))));
    endmodule




**RTL REALIZATION OUTPUT:**

![image](https://github.com/user-attachments/assets/f1282db9-021d-4963-a8a3-0fef89c86975)

FULL SUBTRACTOR:

![image](https://github.com/user-attachments/assets/c5d54b32-547c-4d2b-bb6c-365127085328)



**TIMING WAVEFORM:**

![image](https://github.com/user-attachments/assets/30c3fcdd-10f8-42d8-8383-e5c2441a576d)


**RESULT:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.

**DEVELOPED BY: K DHANUSRI POOJA**


**REGISTRATION NO:24011393**



