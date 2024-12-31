Full Adder using Half Adders
This repository explains the construction of a Full Adder using two Half Adders and an OR gate. A Full Adder is a combinational circuit that performs the addition of three binary bits (two input bits and a carry-in bit). By cascading Half Adders and adding an OR gate, we achieve a Full Adder.

Concept
Half Adder
A Half Adder is a combinational circuit with two inputs and two outputs:

Inputs: A, B
Outputs:
Sum (S) = A ⊕ B
Carry (C) = A ∧ B
Full Adder
A Full Adder performs the addition of three bits:

Inputs: A, B, and Carry-In (Cin)
Outputs:
Sum (S) = A ⊕ B ⊕ Cin
Carry-Out (Cout) = (A ∧ B) ∨ (Cin ∧ (A ⊕ B))
Circuit Design
The Full Adder can be constructed using two Half Adders and an OR gate as follows:

First Half Adder: Takes inputs A and B and generates an intermediate sum and carry.

Outputs:
Intermediate Sum = A ⊕ B
Intermediate Carry = A ∧ B
Second Half Adder: Takes the intermediate sum and Cin as inputs to produce the final sum and a carry-out.

Outputs:
Final Sum = (A ⊕ B) ⊕ Cin
Carry2 = (A ⊕ B) ∧ Cin
OR Gate: Combines the carry outputs of the two Half Adders to produce the final carry-out.

Output:
Final Carry-Out = Intermediate Carry ∨ Carry2
