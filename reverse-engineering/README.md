# reverse-engineering

file elf\_file

**Code**

* The program code itself (also called “text”)

**Data**

* Static variables, allocated when the program is started

**Heap**

* Dynamically allocated memory using malloc and free
* As more and more memory is allocated, it grows upwards

**Stack**

* Local variables and stack frames
* As you make deeper and deeper function calls, ti grows downwards

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>
