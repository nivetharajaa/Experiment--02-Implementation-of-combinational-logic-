

# Experiment--02-Implementation-of-combinational-logic

 
# AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
 
# Equipments Required:
## Hardware 
PCs, Cyclone II , USB flasher
## Software 
Quartus prime

# Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output. F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

1.AND gate The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB Y= A.B

2.OR gate The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation. Y= A+B

 # Procedure

1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.

# Program:
```
Program to implement the given logic function and to verify its operations in quartus using Verilog programming
module ex02(a,b,c,d,f1);
input a,b,c,d;
output f1;
wire x1,x2,x3,x4,x5;
assign x1=(~a)&(~b)&(~c)&(~d);
assign x2=(a)&(~c)&(~d);
assign x3=(~b)&(c)&(~d);
assign x4=(~a)&(b)&(c)&(d);
assign x5=(b)&(~c)&(d);
assign f1=x1|x2|x3|x4|x5;
endmodule
```
## Output:
## RTL realization
![267676863-d7cbaa2e-0fe1-4151-a79d-7139b8f357d7](https://github.com/nivetharajaa/Experiment--02-Implementation-of-combinational-logic-/assets/120543388/c2347d8d-3e6e-4295-a171-7dcca5d11454)

## Truth table
![267677533-4bc17bff-6cba-4037-894e-e6dcdb69f131](https://github.com/nivetharajaa/Experiment--02-Implementation-of-combinational-logic-/assets/120543388/f1028978-b33f-4317-959c-7b73d7d47488)

## waveform
![267677756-f8e8c841-b91e-4f4e-ad75-93e7d9732e29](https://github.com/nivetharajaa/Experiment--02-Implementation-of-combinational-logic-/assets/120543388/bbd5476b-f9d4-4b7c-88c8-f0d88a9857cf)


# Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
