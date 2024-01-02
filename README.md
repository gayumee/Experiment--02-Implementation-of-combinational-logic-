# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime

## Logic Diagram
![Exp2 f1](https://github.com/gayumee/Experiment--02-Implementation-of-combinational-logic-/assets/149037327/52e26db6-7ba2-47f6-ae2d-51828c118ab7)

## Truth Table:
![Exp2 truthtable](https://github.com/gayumee/Experiment--02-Implementation-of-combinational-logic-/assets/149037327/4a1496f0-6efd-414a-9759-bac11c5aa611)


## Program:
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: T. Gayathri 
RegisterNumber:  212223100007
*/
```module f1(a,b,c,d,F1);
input a,b,c,d;
output F1;
wure p,q,r,s,t;
assign p=(~a&~b&~c&~d);
assign q=(~a&~c&~d);
assign r=(~b&~c&~d);
assign s=(~a&b&c&d);
assign t=(b&~c&d);
assign F1 = p|q|r|s|t;
endmodule 
```
## Timing Diagram
![Exp2 f1 timing](https://github.com/gayumee/Experiment--02-Implementation-of-combinational-logic-/assets/149037327/57c62cb8-1808-4660-b3d5-3816bff2b6f4)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
