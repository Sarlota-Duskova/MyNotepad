# Assembly

Assembler output from C source:

`gcc -S code.c`

**Registers:**

* eip (Instruction pointer) points to the next instruction to be executed
* esp (Stack pointer) points to lowest item on the stack
* ebp (Base pointer) points to top of the current stack frame

**push src**

* ESP moves one word down
* Puts the value in **src** at the current ESP

**pop dst**

* Copies the lowest value on the stack (where ESP is pointing) into **dst**
* ESP moves one word up

**mov src dst**

* Copies the value in **src** into **dst**

eax, ax, ah, al

ebx, bx, bh, bl

ecx, cx, ch, cl

&#x20;edx, dx, dh, dl

{% embed url="https://docs.google.com/presentation/d/1YzGTsKpx4orRNHI3FaZtJCHlaFs6ah-YdbkRw9h3txg/edit#slide=id.g13514aafb96_0_1310" %}

Little Endian is where the value is arranged from the least significant byte to the most significant byte:

![](<../.gitbook/assets/image (1).png>)

Big Endian is where the value is arranged from the most significant byte to the least significant byte.

![](../.gitbook/assets/image.png)
