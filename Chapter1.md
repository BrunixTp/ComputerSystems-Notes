# Tour of Computer Systems

A computer system consists of hardware and systems software that work in order to run application prog  rams.

Despite minor changes the underlying concepts don't, meaning, all systems have similar components that perform similar functions.


## 1.1 Information is Bits + Context

A C program starts out as a source program/source file that the programmer creates with an editor and saves in a text file.

A source file is a sequence of bits, each with a value of 0 or 1, organized in 8-bit chunks, called *bytes*.

Each byte represents a text character in the program.

Most computer Systems represent text characters using the ASCII standard.

A C program is stored in a file as a sequence of bytes. Each byte has an integer value that corresponds to some character.

Files such as hello.c that consist of ASCII characters are known as *text files*. All other files are known as *binary files*

All information in a system is represented as a bunch of bits. The only difference between different data objects is the context in which we view them.

For example, in different contexts, the same sequence of bytes might represent an integer, floating-point number, character string, or machine instruction.

Machine representations of numbers are finite approximations that can behave in unexpected ways.

## 1.2 Programs are translated by other Programs into Different Forms

A C program starts as a high-level C program, as it can be read and understood by human beings in that form.

In order to run hello.c on the system, each statement must be translated by other programs into a sequence of low-level *machine-language instructions*.

These instructions are packaged in a form called an *executable object program* and stored as a binary disk file. Object programs are also referred to as *executable object files*.

The translation from source files to object files is performed by a *compiler driver*

gcc -o hello hello.c
=
hello.c -> Pre-Processor (cpp) -> hello.i -> Compiler (cc1) -> hello.s -> Assembler (as) -> hello.o + printf.o -> Linker (ld) -> hello.exe

The gcc compiler driver reads the source file hello.c and translates it into an executable object
