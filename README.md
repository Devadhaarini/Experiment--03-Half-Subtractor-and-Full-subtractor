# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Developed by:
Devadhaarini.D

## Register Number:
23006001

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor
## Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9](https://user-images.githubusercontent.com/36288975/166112538-58c3bc7c-ee5d-4e6a-ac8d-8e8328efe27a.png)


Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6](https://user-images.githubusercontent.com/36288975/166112541-24c68359-3de8-4674-ae22-8272ffc385ed.png)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure
1.Use module projname(input,output) to start the Verilog programmming.

2.Assign inputs and outputs using the word input and output respectively.

3.Use defined keywords like wire,assign and required logic gates to represent the boolean expression.

4.Use each output to represnt onre for differnce and the other for borrow.

5.End the verilog program using keyword endmodule


## Program:
Half Subtractor:

![Screenshot 2023-12-02 133804](https://github.com/Devadhaarini/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145796552/e8b501b5-1d51-456a-8df3-11017b19b4bc)


Full Subtractor:

![Screenshot 2023-12-02 133821](https://github.com/Devadhaarini/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145796552/c6fab0d5-6be8-4b34-9c6a-3af42e2053f8)


## Truthtable
Half Subtractor:

![image](https://github.com/Devadhaarini/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145796552/ac45d315-8d88-406f-8f41-1bffcaadd76f)

Full Subtractor:

![image](https://github.com/Devadhaarini/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145796552/cc27fa19-5286-4550-a379-6f88f97cc50f)


##  RTL realization
Half Subtractor:

![image](https://github.com/Devadhaarini/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145796552/6e055f12-3b58-47c3-ad16-3475ea67c722)

Full Subtractor:

![image](https://github.com/Devadhaarini/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145796552/07e8a742-076e-46b0-a5cf-5231be853870)


## Timing diagram 
Half Subtractor:

![image](https://github.com/Devadhaarini/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145796552/17f3ce4f-3a8c-4522-a7ed-a0b6b92ef486)

Full Subtractor:

![image](https://github.com/Devadhaarini/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145796552/827f7713-a4b8-4d76-a980-1be96506d837)


## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
