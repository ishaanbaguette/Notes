# CO101 – Programming Fundamentals

## Index
- [Algorithms](#algorithms)
- [Flowcharts](#flowcharts)
- [Pseudocode](#pseudocode)
- [Computer Memory Hierarchy](#computer-memory-hierarchy)
- [Translators & Program Execution](#translators--program-execution)
- [Programming Paradigms](#programming-paradigms)
- [Basic Computer Design](#basic-computer-design)

---

## Algorithms
An **algorithm** is a finite sequence of steps that, when executed, solves a given problem.

**Example – Largest of two numbers**
1. Start
2. Read two numbers `a` and `b`
3. If `a > b` then
    - Print `a is largest`
   Else
    - Print `b is largest`
4. Stop

---

## Flowcharts
A **flowchart** is a graphical representation of an algorithm using symbols.

**Common Symbols**
- Oval → Start/Stop  
- Rectangle → Processing  
- Parallelogram → Input/Output  
- Diamond → Selection/Decision  
- Arrow → Flow of control  

---

## Pseudocode
**Problem**: Student with 5 subjects is Pass if average ≥ 40.

**Pseudocode**:

```
Begin
    Set Total = 0
    Set i = 1

    Repeat steps until i > 5:
        Read Marks
        Total = Total + Marks
        i = i + 1

    Average = Total / 5

    If Average >= 40 then
        Print "Pass"
    Else
        Print "Fail"

End
```

---

## Computer Memory Hierarchy

Registers → Cache → Main Memory (RAM) → Secondary Storage → Tertiary Storage

- As we go down: size ↑, speed ↓, cost per bit ↓  

Fun fact: First computer was **ENIAC**.

---

## Translators & Program Execution

### Languages
- **Machine language** – Binary instructions executed directly by the CPU.  
- **Assembly language** – Symbolic form of machine instructions; requires an **assembler**.  
- **High-level languages** – Human-readable (C, Java, Python); require **compiler** or **interpreter**.

### Translators
| Translator | Input → Output | Execution Style | Example Use |
|------------|----------------|-----------------|-------------|
| **Assembler** | Assembly code → Machine code | Converts once, produces object file | Writing low-level drivers, embedded code |
| **Compiler** | High-level code → Machine code | Translates whole program before execution | C, C++ |
| **Interpreter** | High-level code → Executes line by line | No object file; slower but flexible | Python, JavaScript |

---

### Program Execution Steps
1. **Editor** – Write the source code (e.g., `program.c`).  
2. **Preprocessor** – Handles `#include`, `#define`, and macros before compilation.  
3. **Compiler** – Converts preprocessed code into object code (`.o` or `.obj`).  
4. **Linker** – Combines object code with libraries to create the executable.  
5. **Loader** – Loads the executable into main memory for execution by the CPU.

--- 

## Programming Paradigms

| Aspect | Procedural | Object-Oriented |
|--------|------------|-----------------|
| Focus | Functions | Objects |
| Data Handling | Global vars | Encapsulation, Inheritance, Polymorphism |
| Reusability | Low | High |
| Examples | C, Pascal | Java, C++, Python |

---

## Basic Computer Design
**Basic flow**

Input → Storage → CPU → Output

---

### CPU Parts

Its main components are:

- **Control Unit (CU)**  
  Directs the flow of data and instructions. It tells the memory, ALU, and input/output devices how to respond to instructions.

- **Arithmetic Logic Unit (ALU)**  
  Performs all arithmetic operations (addition, subtraction, multiplication, division) and logical operations (comparisons like `<`, `>`, `=`).

- **Memory Unit (Registers + Cache)**  
  Temporary storage inside the CPU. Registers hold data and instructions currently being processed, while cache speeds up access to frequently used data.

---
