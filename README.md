# VSD_RISC-V_based_internship
1 month Research Internship on VSD Squadron Mini based on RISC-V, board is powered by CH32V003F4U6 chip with 32-bit RISC-V core

### Intern: Vijith S
### **College**: SJB Institute of Technology, Bengaluru
### **LinkedIn**: https://www.linkedin.com/in/vijithsatish/
### **Course Instructor**: Kunal Ghosh

---

<details>
<summary><b>Task 1:</b> Install the RISC-V toolchain using the VDI. Write a simple C program to calculate the sum of numbers from 1 to n, compile it using the GCC compiler, and check the output. Then, compile the same code using the RISC-V GCC compiler to analyze its generated instructions.</summary> 
  
<be>


***WHAT IS RISC-V?***
  
>RISC-V  is an open-standard instruction set architecture (ISA) based on Reduced Instruction Set Computing (RISC) principles.  RISC-V is a free and open architecture. It is designed to be simple, extensible, and modular, making it suitable for various applications, from small embedded systems to high-performance computing.

## 1. Download the Virtual Disk Image and Install it using Oracle VM Box**
![Alt text](images/VirtualBox_workshop_05_12_2024_12_59_00.png)

## 2. Write a simple C program to calculate the sum of numbers from 1 to n**
![Alt text](images/lab1_code.png)

## 3. Compile the C code using the GCC compiler, and check the output**
```
cd
```
open the sum1ton.c code 
```

leafpad sum1ton.c
```
compile it using gcc compiler 
```
gcc sum1ton.c
```
run the code using the ./a.out
```
./a.out
```

![Alt text](images/lab1_terminal.png)

## 4. Compile the C code using the RISC V Processor, and check the output**

  the below command compiles the c program using risc v compiler
  
    riscv64-unknown-elf-gcc -o1 -mabi=lp64 -march=rv64i -o 1ton.o 1ton.c

  This command generates a assembly code for the program

    riscv64-unknown-elf-objdump -d 1ton.o
![Alt text](images/riscv_compiler.png)


