# EXPERIMENT--01-ALP-FOR-8086
## Name :prideesh M
## Roll no :212223040154
## Date of experiment :





## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
org 100H
mov AH,0A2H;
mov BH,0B3H;
add AH,BH;
mov [1554H],AH;
ret
```

## Output  
 ![add](https://github.com/prideeshm/EXPERIMENT--01-ALP-FOR-8086/assets/144870483/00afdc6d-2970-4e31-b144-ea957c56aeb9)

## Subtraction   of 8 bit numbers  ALP 
``` 
org 100H
mov AH,0C4H;
mov BH,0B2H;
sub AH,BH;
mov [1424h],AH;
ret
```
## Output 
![sub](https://github.com/prideeshm/EXPERIMENT--01-ALP-FOR-8086/assets/144870483/549545bd-b4e3-4da2-8c4b-f24d99827714)

## Multiplication alp 
```
org 100H
mov AL,0C4H;
mov BL,0B2H;
mul BL;
mov [1334H],AX;
ret
```
 ## Output  
![mul](https://github.com/prideeshm/EXPERIMENT--01-ALP-FOR-8086/assets/144870483/7143d472-7c80-475d-a6d1-798f7568afe5)


## Division alp 

```
org 100H
mov AL,0D5H;
mov BL,0A2H;
div BL;
mov [1364H],AX;
ret
```
## Output  
![div](https://github.com/prideeshm/EXPERIMENT--01-ALP-FOR-8086/assets/144870483/8ba094b2-bd6a-44bf-9088-fbec96bda98d)

## program for logical operations
```
org 100H
MOV SI,0532H;
MOV AX,0A32H;
MOV BX,0B13H;
OR AX,BX;
MOV [SI],AX;
MOV AX,0A32H;
MOV BX,0B13H;
AND AX,BX;
MOV [SI+2],AX;
MOV AX,0A32H;
MOV BX,0B13H;
XOR AX,BX;
MOV [SI+4],AX;
MOV AX,0A32H;
NOT AX;
MOV [SI+6],AX;
ret
```
## output
![logical](https://github.com/prideeshm/EXPERIMENT--01-ALP-FOR-8086/assets/144870483/8a000bac-5c28-4385-a6f5-207d56e35e2b)

## Result :
Thus, a program is executed on ALP for the fundamental arithmetic and logical operations.








