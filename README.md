### study-of-basic-gates

**AIM:** 

To study and verify the truth table of logic gates in Quartus II using Verilog programming.

**Equipments Required:**

Software – Quartus prime 

**Theory**

Introduction Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as

AND gate OR gate NOT gate NAND gate NOR gate Ex-OR gate Ex-NOR gate

**AND gate**

The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB
Y= A.B

**OR gate** 

The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation.
Y= A+B

**NOT gate**

The NOT gate is an electronic circuit that produces an inverted version of the input at its output. It is also known as an inverter. If the input variable is A, the inverted output is known as NOT A. This is also shown as A' or A with a bar over the top, as shown at the outputs.
Y= A'

**NAND gate**

This is a NOT-AND gate which is equal to an AND gate followed by a NOT gate. The outputs of all NAND gates are high if any of the inputs are low. The symbol is an AND gate with a small circle on the output. The small circle represents inversion.
Y= (AB)’

**NOR gate**

This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.
Y= (A+B)’

**Ex-OR gate**

The 'Exclusive-OR' gate is a circuit which will give a high output if either, but not both of its two inputs are high. An encircled plus sign (⊕) is used to show the Ex-OR operation.
Y= A⊕B

**Ex-NOR gate**

The 'Exclusive-NOR' gate circuit does the opposite to the EX-OR gate. It will give a low output if either, but not both of its two inputs are high. The symbol is an EX-OR gate with a small circle on the output. The small circle represents inversion.
Y= A⊕B

**Procedure** 

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**PROGRAM**

Program for logic gates and verify its truth table in quartus using Verilog programming
```
module basic_gates(
    input A, B,
    output y0, y1, y2, y3, y4, y5
);

and  g0 (y0, A, B);
or   g1 (y1, A, B);
not  g2 (y2, A);
nand g3 (y3, A, B);
nor  g4 (y4, A, B);
xor  g5 (y5, A, B);`

endmodule
```
 Developed by: SATHISH S RegisterNumber: 212225040390
 
**Logic symbol & Truthtable**
<img width="358" height="674" alt="image" src="https://github.com/user-attachments/assets/6251d7a6-a1e4-423e-9465-7f928fbf4de7" />


**RTL realization Output:**
<img width="891" height="713" alt="Screenshot 2026-03-12 213812" src="https://github.com/user-attachments/assets/632d939b-e90c-40dd-89bc-4565553ea7c7" />


**RTL**
<img width="1322" height="764" alt="Screenshot 2026-03-12 215854" src="https://github.com/user-attachments/assets/877a9b53-70c8-4cb8-a9cd-7077b2c36e98" />

**Result:**
The Truth table of logic gates in Quartus II using Verilog programming is verified.
