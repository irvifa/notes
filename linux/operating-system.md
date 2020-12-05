# Operating System (OS)

Collection of system programs which allow the user to run application software. Usually it will
provides abstractions for applications such as:

- manages and hides details of hardware
- accesses hardware through low level interfaces unavailable through applications'

## Memory management

OS has the basic ability to fool the software running in the system into
believing that it is running in a lot of memory. This is done by make a small
amount of physical memory behave like rather more memory, known as virtual memory.

## Processes

Process is a running program, each process is a separate entity that is running a particular program.
We can see available processes by using `ps` command. The OS is running each process in turn for a short period, 
known as a time-slice.
A process is logically divided into the following parts, known as segments:
- Text: the instructions of the program.
- Data: the static variables used by the program.
- Heap: an area from which programs can dynamically allocate extra memory.
- Stack: a piece of memory that grows and shrinks as functions are called and
return and that is used to allocate storage for local variables and function call
linkage information.

Processes are protected from one another, by giving each process a separate address space which only they have access to.

## Device Driver

Device drivers make up the major part of the Linux kernel.
Device drivers control the interaction between the operating system and the hardware device that they are controlling. 

## Filesystem

A filesystem gives the user a sensible view of files and directories held on the hard disks of the system regardless of the filesystem type.

## Kernel Data Structures
 
 The operating system must keep a lot of information about the current state of the system. As things happen within the system these data structures must be changed to reflect the current reality.
 
 - Linked List
 - Hash Tables, e.g. cache implementation
 - Abstract Interfaces, e.g. network device drivers have interfaces with different implementation for certain routines
