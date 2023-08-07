---
Date: 07-20-2023
---
The [[CPU]]'s memory that is faster to use than  [[RAM]] however can hold an extremally small amount of data.

In a [[CPU]] with [[32-Bit Architecture]] each register can hold 32 [[bits]]

In a [[CPU]] with [[64-Bit Architecture]] each register can hold 64 [[bits]]

On a [[32-Bit Architecture]] there are four registers that each hold 32 [[bits]]:
- EAX
- EBX
- ECX
- EDX

AX allows for the lower 16 bits AL allows for the lower 8 bits of AX and AH allows for the higher 8 bits of AX  [^1]


[^1]: This is the same for the others for example BX would get the lower 16 bits of EBX
there are also registers which cannot be accessed with AH or AL but still with AX:
- ESP:stack pointer
- EBP:base pointer
- ESI: Source index
- EDI: Destination Index

There are also some registers to be used by programs:
- EIP: Instructional Pointer memory address of next instruction.