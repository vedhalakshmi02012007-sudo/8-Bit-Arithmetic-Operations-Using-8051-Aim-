# 8-Bit-Arithmetic-Operations-Using-8051

## Aim:
To perform 8-bit arithmetic operations such as addition, subtraction, multiplication, and division using the 8051 microcontroller.

## Apparatus Required:

•	Laptop with Keil uVision software

## Algorithm:

## For Addition:
1.	Load the first number from memory location 30H into register A.
2.	Load the second number from memory location 31H into register B.
3.	Add the contents of registers A and B.
4.	Store the result in memory location 40H.
5.	Store the carry (if any) in 41H.

## Program:
ORG 0000H;<br>
MOV  A,30H;<br>
ADD A,31H;<br>
MOV 40H,A;<br>
JNC NEXT;<br>
MOV 41H,#01H;<br>
SJMP END_PROGRAM;<br>
NEXT:MOV 41H,#00H;<br>
END_PROGRAM:NOP;<br>
END<br>


## Output:
<img width="1914" height="1114" alt="Screenshot 2025-10-27 133551" src="https://github.com/user-attachments/assets/252dac63-1e62-423e-a4d3-d84710fad662" />

<img width="952" height="181" alt="Screenshot 2025-10-27 133616" src="https://github.com/user-attachments/assets/0398e102-27b8-4150-a895-4769be04faa1" />

<img width="235" height="491" alt="Screenshot 2025-10-27 133633" src="https://github.com/user-attachments/assets/f4eaf3ea-54a9-4e6c-ade5-d0281d5a1c71" />



   
## For Subtraction:
1.	Load the first number from memory location 30H into register A.
2.	Load the second number from memory location 31H into register B.
3.	Subtract B from A.
4.	Store the result in memory location 40H.

## Program:
ORG 0000H;<br>
MOV A,30H;<br>
SUBB A,31H;<br>
MOV 40H,A;<br>
JNC NEXT ;<br>
MOV 41H,#01H;<br>
SJMP END_PROGRAM;<br>
NEXT:MOV 41H,#00H;<br?
END_PROGRAM:NOP;<br>
END<br>




## Output:

<img width="1917" height="1106" alt="Screenshot 2025-10-27 141609" src="https://github.com/user-attachments/assets/2c8f3221-8e37-4240-ba31-f8173fbff4df" />


<img width="952" height="188" alt="Screenshot 2025-10-27 141653" src="https://github.com/user-attachments/assets/bda8b908-be0d-4326-afed-9d757426cbf4" />


<img width="241" height="452" alt="Screenshot 2025-10-27 141705" src="https://github.com/user-attachments/assets/0ac3a052-85f6-4305-a961-4ead14523449" />




## For Multiplication:
1.	Load the first number from memory location 30H into register A.
2.	Load the second number from memory location 31H into register B.
3.	Multiply A and B.
4.	Store the lower byte of the result in memory location 40H.
5.	Store the higher byte of the result in memory location 41H.

## Program:
ORG 0000H;<br.
MOV A,30H;<br>
MOV B,31H;,br>
MUL AB;<br>
MOV 40H,A;<br>
MOV 41H,B;<br>
END<br>


## Output:

<img width="1914" height="1091" alt="Screenshot 2025-10-27 143240" src="https://github.com/user-attachments/assets/bde9da2c-3c5d-4b29-a544-2637362e511f" />


<img width="953" height="271" alt="Screenshot 2025-10-27 143311" src="https://github.com/user-attachments/assets/e503d9d9-9e77-4fa3-8f1f-e09c4305eb1a" />


<img width="242" height="490" alt="Screenshot 2025-10-27 143321" src="https://github.com/user-attachments/assets/ace8e3f3-ed16-4d6e-b27c-5527b79bafe4" />





## For Division
1.	Load the dividend from memory location 30H into register A.
2.	Load the divisor from memory location 31H into register B.
3.	Divide A by B.
4.	Store the quotient in memory location 40H.
5.	Store the remainder in memory location 41H.


## Program:
ORG 0000H;<br>
MOV A,30H;,br>
MOV B,31H;<br>
DIV AB;<br>
MOV 40H,A;<br>
MOV 41H,B;<br>
END<br>


## Output:

<img width="1916" height="1098" alt="Screenshot 2025-10-27 144626" src="https://github.com/user-attachments/assets/ce87ffe5-f9f7-44a2-b9ab-c64ee1906f4f" />

<img width="955" height="270" alt="Screenshot 2025-10-27 144650" src="https://github.com/user-attachments/assets/397ca9b3-e8c8-4b15-8f8e-3943f4fe14b8" />


<img width="238" height="546" alt="Screenshot 2025-10-27 144701" src="https://github.com/user-attachments/assets/9fc50952-60c2-4c59-8042-b82f87083b9a" />







## Result:
The 8-bit arithmetic operations using the 8051 microcontroller have been successfully executed and verified using Keil software.

