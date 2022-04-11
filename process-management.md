A process is an abstraction for a running program.

the goal of a process is to :

1. give each process a private memory area for code, data, stack

2. prevent one process from reading/writing outside its adress space.

the implementation is split between the O/S and the hardware.

the O/S part:

1. allocate physical memory for processes (creating, extension, deletion)

2. keep track of them when they are not executing.

3. switch between processes.

the hardware:

1. translate user addresses to physical addresses.

2. detect and prevent attempts to use memory outside the address space.

3. allow cross-space transfers (system calls, interrupts)

