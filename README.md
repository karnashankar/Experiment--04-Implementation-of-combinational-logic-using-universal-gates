# Experiment--04-Implementation-of-combinational-logic-using-universal-gates
Implementation of combinational logic using universal-gates
 
## AIM:
To implement the given logic function using NAND and NOR gates and to verify its operation in Quartus using Verilog programming.

F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate
F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')' using NOR gate
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output. 

## Using NAND gates
NAND gate is actually a combination of two logic gates i.e. AND gate followed by NOT gate. So its output is complement of the output of an AND gate.This gate can have minimum two inputs, output is always one. By using only NAND gates, we can realize all logic functions: AND, OR, NOT, X-OR, X-NOR, NOR. So this gate is also called as universal gate. First note that the entire expression is inverted and we have three terms ANDed. This means that we must use a 3-input NAND gate. Each of the three terms is, itself, a NAND expression. Finally, negated single terms can be generates with a 2-input NAND gate acting as an inverted.

F=((C'.B.A)'(D'.C.A)'(C.B'.A)')'

## Logic Diagram

Using NOR gates
NOR gate is actually a combination of two logic gates: OR gate followed by NOT gate. So its output is complement of the output of an OR gate. This gate can have minimum two inputs, output is always one. By using only NOR gates, we can realize all logic functions: AND, OR, NOT, Ex-OR, Ex-NOR, NAND. So this gate is also called universal gate. Designing a circuit with NOR gates only uses the same basic techniques as designing a circuit with NAND gates; that is, the application of deMorgan’s theorem. The only difference between NOR gate design and NAND gate design is that the former must eliminate product terms and the later must eliminate sum terms.

F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')'

## Logic Diagram
## Procedure
##### STEP 1:Create a project with required entities.
##### STEP 2:Create a module along with respective file name.
##### STEP 3:Run the respective programs for the given boolean equations.
##### STEP 4:Run the module and get the respective RTL outputs.
##### STEP 5:Create university program(VWF) for getting timing diagram.
##### STEP 6:Give the respective inputs for timing diagram and obtain
## Program:

##### Program to implement the given logic function using NAND and NOR gates and to verify its operations in quartus using Verilog programming.
##### Developed by: karna s
##### RegisterNumber:22008977  
#### Using NAND gate
<img width="641" alt="image" src="https://user-images.githubusercontent.com/121109150/214824889-4c204299-0539-4c60-b09b-c1beb1e09c5f.png">
 
 #### Using NOR gate
<img width="604" alt="image" src="https://user-images.githubusercontent.com/121109150/214825009-8049940f-62b0-4b7d-9e56-fc58b721cb65.png">

## Output:
### Using NAND gate
##### RTL
![image](https://user-images.githubusercontent.com/121109150/214825806-c60afa45-c32b-47f8-947e-ec2d980e5003.png)

##### Timing Diagram
<img width="669" alt="image" src="https://user-images.githubusercontent.com/121109150/214826004-1fa2e131-a9e9-4e7f-8c05-cdbd070ab33a.png">


##### Truth Table:
![image](https://user-images.githubusercontent.com/121109150/214826053-e541c2b6-73a1-492c-b696-0c2b9e5bc2c5.png)

 ### Using NOR gate
##### RTL
![image](https://user-images.githubusercontent.com/121109150/214826203-6cad663b-0d19-4693-9049-ce8ebd7b816a.png)

##### Timing Diagram
<img width="661" alt="image" src="https://user-images.githubusercontent.com/121109150/214826330-36eaa55a-6699-4de1-88f0-7991235ca4a6.png">


##### Truth Table:
<img width="667" alt="image" src="https://user-images.githubusercontent.com/121109150/214826434-93bf051f-3c56-48e4-89ce-6cfa385c5c92.png">

## Result:
Thus the given logic functions are implemented using NAND and NOR gates and their operations are verified using Verilog programming.
