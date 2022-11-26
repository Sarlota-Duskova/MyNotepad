# ARM Assembly

{% embed url="https://cpulator.01xz.net/?sys=arm-de1soc" %}

### Registers

![](../.gitbook/assets/image.png)

Each zero represents a single hexadecimal value, that value represent four bits of data so we have in total 32 bits that we can work with.

* Registers from r0 to r6 is for general purpose.
* r7 has a special functionality to system calls, when we want to call to the operating system to do something for us, so we will store that numerical value in register r7
* **sp register (stack pointer)**, stack memory is stored in the RAM of the computer. It is slower to access and slower to write to it.
* **lr register (link register)** it stores the location that a function should return back to (it is like in high level language, function with return, move back to the location of what called the function)&#x20;
* pc register (program counter)
* **cpsr register** to store information about our program, for example if we store information about that number is negative
* spsr register&#x20;







Starting point of applicaition:

```armasm
.global _start
_start:
```

```armasm
.global _start
_start:
// FIRST PROGRAM
	MOV R0,#30 // move 30 decimal to register R0
	MOV R7,#1 // #1 will exit that program 
	SWI 0 // SWI software interrupts, lets the OS take over
```

```armasm
.global _start
_start:
// SECOND PROGRAM
	LDR R0,=list //LDR = load data from stuck into register
	LDR R1,[R0] //[] = will tell what value is associate in R0 register
	LDR R2,[R0,#4]! //! = increment comes afterward
.data 
list:
	.word 4,5,-9,1,0,2,-3 //.word mean it will be 32bits
```

























