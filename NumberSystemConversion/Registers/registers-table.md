# CPU Registers - Complete Table

| **Register** | **Overview** | **Type** | **Technical Example** | **Code Example** |
|--------------|--------------|----------|------------------------|-------------------|
| **AX (Accumulator)** | Primary accumulator for arithmetic & I/O operations | General Purpose | Add two numbers, result stored in AX | `MOV AX, 5` <br> `ADD AX, 3` |
| **BX (Base)** | Often used as base address pointer for memory addressing | General Purpose | Used in indexed addressing | `MOV BX, 1000h` <br> `MOV AX, [BX]` |
| **CX (Counter)** | Counter for loops and string operations | General Purpose | Used as loop counter in LOOP instruction | `MOV CX, 5` <br> `LOOP start` |
| **DX (Data)** | Holds data for I/O operations, also used in multiplication/division | General Purpose | Used with AX in 32-bit multiplication | `MOV DX, 0` <br> `MUL BX` |
| **SI (Source Index)** | Source index for string operations | Pointer/Index | Points to source in string copy | `MOV SI, OFFSET src` |
| **DI (Destination Index)** | Destination index for string operations | Pointer/Index | Points to destination in string copy | `MOV DI, OFFSET dest` |
| **BP (Base Pointer)** | Points to base of stack frame for parameter access | Pointer/Index | Used to access function arguments on stack | `MOV AX, [BP+4]` |
| **SP (Stack Pointer)** | Points to top of stack | Pointer/Index | Changes with PUSH/POP | `PUSH AX` <br> `POP BX` |
| **IP (Instruction Pointer)** | Points to next instruction to execute | Special Purpose | Automatically incremented | (Not directly accessible) |
| **FLAGS** | Stores status flags (zero, carry, overflow, etc.) | Special Purpose | Check after arithmetic | `CMP AX, BX` <br> `JE equal_label` |