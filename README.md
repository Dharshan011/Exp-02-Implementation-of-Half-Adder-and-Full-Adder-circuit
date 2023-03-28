# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
```
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: DHARSHAN V
RegisterNumber: 212222230031
=======
## Half adder program:

module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule

## Full adder program:

module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
*/
```
## OUTPUT:
## Logic symbol & Truthtable
HALF ADDER
![Screenshot 2023-03-28 160933](https://user-images.githubusercontent.com/113497491/228211024-a93d75e9-c241-4afc-bf61-4f257dbddc9f.png)
FULL ADDER
![Screenshot 2023-03-28 160944](https://user-images.githubusercontent.com/113497491/228211072-f9fac99a-0c6d-4d4d-9a25-27ae9a6f73d1.png)

## RTL realization
HALF ADDER
![WhatsApp Image 2023-03-27 at 9 33 30 AM](https://user-images.githubusercontent.com/113497491/228211455-6b867b83-512d-4ffc-bd42-b9a5334356f6.jpeg)

FULL ADDER
![WhatsApp Image 2023-03-27 at 9 19 37 AM](https://user-images.githubusercontent.com/113497491/228211367-f2d2f570-44df-4d8d-985d-913d83a8f441.jpeg)

### TIMING DIAGRAM
HALF ADDER
![WhatsApp Image 2023-03-27 at 9 47 09 AM](https://user-images.githubusercontent.com/113497491/228211593-db89f8ef-84cd-4a3b-85f0-62ff352b5582.jpeg)
FULL ADDER
![WhatsApp Image 2023-03-27 at 9 23 29 AM](https://user-images.githubusercontent.com/113497491/228211694-6075fbdc-8ea7-4c90-aaa6-7381356046bf.jpeg)

### TRUTH TABLE 

HALF ADDER


![Screenshot 2023-03-28 161343](https://user-images.githubusercontent.com/113497491/228211978-48d2b7f3-437f-4cba-8cfe-13da6861617c.png)


FULL ADDER

![Screenshot 2023-03-28 161348](https://user-images.githubusercontent.com/113497491/228212028-db53ad67-0d8c-45e6-a469-bcb5f60e9bb8.png)
### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified
