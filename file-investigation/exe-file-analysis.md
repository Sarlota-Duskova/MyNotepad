# EXE file Analysis

`hexdump -C filename.exe`

`less filename.exe`

**ExifTool**

`apt intall -y exiftool`

**Objdump**

`objdump -f filename.exe`

`objdump -d filename.exe`

**Strings**

`strings filename.exe`

To show only 6-byte or greater strings (from lecture):

`strings -n 6 filename.exe`

To show any UTF-16 “Little Endian” strings, again with minimum length 16. This is very handy for Windows binaries, as many of them have UTF-16 string contents:

`strings -n 6 -e l filename.exe`

If you want `strings` to also report the offset (within the file on disk) of each string, you may use the `-t x` option, which will report this offset from the beginning of the file in hexadecimal.

`strings -n 6 -e l -t x filename.exe`
