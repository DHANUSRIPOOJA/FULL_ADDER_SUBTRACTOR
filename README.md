# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**EQUIPMENTS REQUIRED:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**FULL ADDER AND FUL SUBTRACTOR:**

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

**TRUTHTABLE:**

FULL ADDER:

![image](https://github.com/user-attachments/assets/1a684bf1-effd-46ae-b98e-de89eea34dfc)


FULL SUBTRACTOR:

![image](https://github.com/user-attachments/assets/8e72d622-1fd2-4479-b97e-46b16f12d190)

**PROCEDURE:**

1. Type the program in Quartus software.
2. Compile and run the program.
3. Generate the RTL schematic and save the logic diagram.
4. Create nodes for inputs and outputs to generate the timing diagram.
5. For different input combinations generate the timing diagram.


**PROGRAM:**

    module ha(a,b,sum,carry);
    input a,b;
    output sum,carry;
    assign sum= (a ^ b);
    assign carry= ( a & b);
    endmodule


    module hs(a,b,difference,borrow);
    input a,b;
    output difference,borrow;
    assign difference= (a ^ b);
    assign borrow= ( ~a & b);
    endmodule

**RTL REALIZATION OUTPUT:**

FULL ADDER:

![Screenshot 2024-12-25 210853](https://github.com/user-attachments/assets/1cd25bf8-df9a-4f74-a149-e71f3cd5fdae)

FULL SUBTRACTOR:

![Screenshot 2024-12-25 210939](https://github.com/user-attachments/assets/58a7180c-e1ad-460b-974a-1d0f22041f7e)

**TIMING WAVEFORM:**

![Screenshot 2024-12-25 211045](https://github.com/user-attachments/assets/738eecea-a635-4a83-9903-bf95b8ad2661)

**RESULT:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.

DEVELOPED BY: K DHANUSRI POOJA
REGISTER NNUMBER:24011393



