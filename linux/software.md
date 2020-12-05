# Software

## Language, Operating System, and Memory management

Program: A set of computer instruction to perform a task

Instructions fetched by CPU aren't understandable by humans. The instruction will depend on the architecture, 
for example 0x89E5 is an Intel 80486 instruction which copies the contents of the ESP register to the EBP register.

Writing code in Assembly language is difficult and error prone for human. Another downside of this language
is the fact that it's not portable and tightly coupled with the architecture, hence there's a language more
suitable for human being, e.g. C. Compilers will read the language and translate it into assembly.
C supports many types of variables, a variable is a location in memory which can be referenced by a symbolic name. 
User, in this case programmer doesn't care where the variable stored, it is linker's job.
Pointers are variables that contain the address, the location in memory of other data.

PS:
- The register ESP (literally "extended stack pointer") holds the top of the stack. This is the point where the instructions which use the stack (PUSH, POP, CALL and RET) actually use the stack.
- The register EBP (literally "extended base pointer") is traditionally moved by the programmer to a particular place on the stack at any one time, so that data on the stack can be read from and written to using base index addressing.

Linkers are programs that link together several object modules and libraries to form a single, coherent, program.
Object modules are the machine code output from an assembler or compiler and contain executable machine code and data together with information that allows the linker to combine the modules together to form a program.
