# Unallocated Memory Segment Access in Assembly

This repository demonstrates a common yet subtle error in assembly programming: attempting to access a memory segment that has not been properly allocated.  This can manifest as program crashes, unexpected behavior, or data corruption.

The `bug.asm` file contains the erroneous code. The `bugSolution.asm` file provides a corrected version, illustrating how to properly allocate and access memory segments.

## How to reproduce the bug:
1. Assemble and link `bug.asm`.
2. Run the resulting executable.
3. Observe the program's termination or unexpected behavior.

## Understanding the solution:
The solution involves ensuring that memory segments are allocated before they're accessed.  This typically involves using operating system calls or memory management functions (depending on the specific assembly environment).