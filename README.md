# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
```
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: MANOJ G
RegisterNumber:  212222240060
/*
Program to implement the given logic function using NAND and NOR gates and to verify its operations in quartus using Verilog programming.
module cpmbine(a,b,c,d,f);
input a,b,c,d;
output f;
wire p,q,r;
assign p=(~c & b & a);
assign q=(~d & c & c & a);
assign r=(c & ~b & a);
assign f=(~(~p & ~q & ~r));
endmodule

module combine1(a,b,c,d,f);
input a,b,c,d;
output f;
wire p,q,r;
assign p=(c & ~b & a);
assign q=(d & ~c & a);
assign r=(c & ~b & a);
assign f=((p | q & |r));
endmodule
```

*/
## RTL realization

## Output:
## RTL
![image](https://user-images.githubusercontent.com/69635071/234762464-e0c1ec80-46a9-461c-924c-0b8563dd97ee.png)


![image](https://user-images.githubusercontent.com/69635071/234762543-5b9a7466-b7f6-4091-b651-b4f1cbbbbe3a.png)




## Timing Diagram
![image](https://user-images.githubusercontent.com/69635071/234762646-95ed6679-471c-4b42-9a1b-58146125ad02.png)
![image](https://user-images.githubusercontent.com/69635071/234762744-c5146d6d-0d43-48c0-8f3e-6aa8aaca979c.png)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
