# Creating-and-a-kernel-and-its-implementation-
Creating an operating system (OS) kernel is essentially building the core foundation of an operating system. It's the program that directly interacts with the computer's hardware and provides essential services for other programs to run 


The first part of writing an operating system is to write a bootloader in 16 bit assembly (real mode).
Bootloader is a piece of program that runs before any operating system is running.
it is used to boot other operating systems, usually each operating system has a set of bootloaders specific for it.
Bootloaders generally select a specififc operating system and starts it's process and then operating system loads itself into memory.

**Requirements**
GNU/Linux :-  Any distribution(Ubuntu/Debian/RedHat etc.).
Assembler :-  GNU Assembler(gas) to assemble the assembly laguage file.
GCC :-  GNU Compiler Collection, C compiler. Any version 4, 5, 6, 7, 8 etc.
Xorriso :-  A package that creates, loads, manipulates ISO 9660 filesystem images.(man xorriso)
grub-mkrescue :-  Make a GRUB rescue image, this package internally calls the xorriso functionality to build an iso image.
QEMU :-  Quick EMUlator to boot our kernel in virtual machine without rebooting the main system.

**Using the code**
Writing a kernel from scratch is to print something on screen.
So we have a VGA(Visual Graphics Array), a hardware system that controls the display.

**Implementation **
1. Keyboard
2. Ping Pong
