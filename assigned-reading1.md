# Reading Notes

## 1.3

- Great example of abstraction is the process of going from application code to hardware instructions
- **Systems software:** Software that provides services that are commonly useful, including operating systems, compilers, loaders, and assemblers.
- **Operating system:** Supervising program that manages the resources of a computer for the benefit of the programs that run on that computer.
  - Handling basic input and output operations
  - Allocating storage and memory
  - Providing for protected sharing of the computer among multiple applications using it simultaneously
- **Compiler:** A program that translates high-level language statements into assembly language statements.
  - Example: the process of how say a java gui app code can turn into instructions for the hardware
- Binary digit: Also called a bit. One of the two numbers in base 2 (0 or 1) that are the components of information.
- **Instruction:** A command that computer hardware understands and obeys.
- **Assembler:** A program that translates a symbolic version of instructions into the binary version.  
- Assembly language: A symbolic representation of machine instructions
- **Machine language:** A binary representation of machine instructions.
- **High-level programming language:** A portable language such as C, C++, Java, or Visual Basic that is composed of words and algebraic notation that can be translated by a compiler into assembly language.

## 2.4

- **Binary digit:** Also called a bit. One of the two numbers in base 2 (0 or 1) that are the components of information.
- **Least significant bit:** The rightmost bit in a MIPS word.
- **Most significant bit:** The leftmost bit in a MIPS word..
- **Overflow:** when the results of an operation are larger than can be represented in a register.
- **Two's complement:** A signed number representation where a leading 0 indicates a positive number and a leading 1 indicates a negative number. The complement of a value is obtained by complementing each bit (0 → 1 or 1 → 0), and then adding one to the result (explained further below)
- **One's complement:** A notation that represents the most negative value by 10 … 000two and the most positive value by 01 … 11two, leaving an equal number of negatives and positives but ending up with two zeros, one positive (00 … 00two) and one negative (11 … 11two). The term is also used to mean the inversion of every bit in a pattern: 0 to 1 and 1 to 0.
- **Biased notation:** A notation that represents the most negative value by 00 … 000two and the most positive value by 11 … 11two, with 0 typically having the value 10 … 00two, thereby biasing the number such that the number plus the bias has a non-negative representation.

## 3.2

### Overflow table guide

| Operation| Operand A| Operand B| Result Indicating overflow|
| ---------| ---------| ---------| --------------------------|
| A+B      | $\geq 0$ | $\geq 0$ | $<0$|
| A+B      | $<0$     | $<0$     | $\geq 0$    |
| A-B      | $\geq 0$ | $<0$     | $\leq 0$    |
| A-B      | $<0$     | $\geq 0$ | $\geq 0$    |

- **Arithmetic Logic Unit (ALU):** Hardware that performs addition, subtraction, and usually logical operations such as AND and OR.
- **Exception:** Also called interrupt on many computers. An unscheduled event that disrupts program execution; used to detect overflow, for example. 
- **Interrupt:** An exception that comes from outside of the processor. (Some architectures use the term interrupt for all exceptions.)
- 