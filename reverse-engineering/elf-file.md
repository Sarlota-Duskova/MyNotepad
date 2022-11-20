# ELF file

For changing binary:

`hexedit file`&#x20;

Check file header:

`file file`

Check assembly data:

`r2 file`

`aaa` analyze

`s main` search for main &#x20;

`pdf` show a disassembly

### GDB debugger

`gdb file`

List different functions in the binary file:

`(gdb) info functions`

Set a **breakpoint** at the memory address of this function:

`(gdb) b *0x0000000000400520`

Run the binary in gdb with some test input:

`(gdb) run test`

View the current state of the registers:

`(gdb) info registers`

Print the strings at these addresses:

`(gdb) x/s 0x7fffffffe030`

### Ghidra



