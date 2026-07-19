# Introduction to Information Technology — Study Notes



#### 1.1.3 Working of a Computer

**Theory**
The working of a computer can be compared to operating a television: switch on the TV, connect antenna/set-top box (input), change channel and adjust volume (processing), and view the programme on screen (output). Similarly, computers require both hardware and software to operate. The block diagram shows three functional units — Input unit, Central Processing Unit (CPU), and Output unit — with the CPU further divided into Control Unit (CU), Arithmetic and Logic Unit (ALU), and Memory Unit.

**Important Points**

| Unit | Role |
|------|------|
| **Input Unit** | Receives data/instructions from outside world (keyboard, mouse, camera, mic) |
| **Control Unit (CU)** | Coordinates operations using timing signals from CPU clock; determines instruction execution order |
| **ALU** | Performs arithmetic (add, subtract, multiply, divide) and logical (AND, OR, NOT) operations |
| **Memory Unit** | Stores data, instructions during processing, and results for future use |
| **Output Unit** | Delivers processed data/results to user in desired form |

- TV analogy: hardware = TV components; channels = software
- CPU is the brain of the computer; all processing happens here

**For Exam**
A computer works through three functional units: Input unit (receives data from outside), CPU (processes data using Control Unit for coordination, ALU for calculations, and Memory Unit for temporary storage), and Output unit (delivers results to the user). Both hardware and software are required for proper functioning, similar to how a TV needs both physical components and broadcast channels.

**Diagram (refer SLM):** Fig. 1.1.2 Block diagram of a digital computer — Input unit, CPU (CU, ALU, Memory Unit), Output unit.

#### 1.1.4 Von-Neumann Model 🔥

**Theory**
In 1945, John Von Neumann proposed a computer architecture concept known as Von-Neumann Architecture. This architecture consists of Control Unit, ALU, registers, memory unit, and input/output unit. Its key feature is the stored program concept — both data and programs reside in the same memory, enabling modern general-purpose computing where instructions and data are treated uniformly in memory.

**Important Points**

- Proposed by **John Von Neumann in 1945**
- Components: CU, ALU, registers, memory unit, I/O unit
- **Stored program concept:** data and programs in same memory
- Foundation of modern computer architecture
- Enables sequential instruction execution from memory

**For Exam**
Von-Neumann Architecture (1945, John Von Neumann) consists of Control Unit, ALU, registers, memory unit, and I/O unit. Its key feature is the stored program concept — both data and programs reside in the same memory, enabling modern general-purpose computing. This design became the foundation for virtually all modern computers.


### Unit 2: Number Systems and Codings

#### 1.2.1 Number Systems 🔥

**Theory**
Computers understand only the language of numbers — machine language uses binary values 0 and 1. IC chips operate on two voltage states (presence = 1, absence = 0), so the base-2 binary number system is fundamental. A number system is a mathematical notation for representing numbers using symbols and digits consistently; the base or radix defines how many unique digits can occur in each position. Besides binary (base-2), programmers also use octal (base-8) and hexadecimal (base-16) to represent binary data more concisely.

**Important Points**

| System | Base | Digits/Symbols | Key Terms |
|--------|------|----------------|-----------|
| **Binary** | 2 | 0, 1 | Bit (1 digit), Nibble (4 bits), Byte (8 bits), MSB, LSB |
| **Decimal** | 10 | 0–9 | MSD (leftmost), LSD (rightmost); positional weights in powers of 10 |
| **Octal** | 8 | 0–7 | Base 8 = 2³; each octal digit = 3-bit binary group |
| **Hexadecimal** | 16 | 0–9, A–F | Base 16 = 2⁴; each hex digit = 4-bit binary group; compact binary representation |

**Decimal to Binary Conversion (Repeated Division by 2)**

| Decimal | Binary | Decimal | Binary |
|---------|--------|---------|--------|
| 0 | 0 | 8 | 1000 |
| 1 | 1 | 9 | 1001 |
| 2 | 10 | 10 | 1010 |
| 3 | 11 | 15 | 1111 |
| 4 | 100 | 16 | 10000 |
| 5 | 101 | 50 | 110010 |
| 6 | 110 | 101 | 1100101 |
| 7 | 111 | 1000 | 1111101000 |

**Decimal ↔ Hex ↔ Binary (0–15)**

| Dec | Binary | Hex | Dec | Binary | Hex |
|-----|--------|-----|-----|--------|-----|
| 0 | 0000 | 0 | 8 | 1000 | 8 |
| 1 | 0001 | 1 | 9 | 1001 | 9 |
| 2 | 0010 | 2 | 10 | 1010 | A |
| 3 | 0011 | 3 | 11 | 1011 | B |
| 4 | 0100 | 4 | 12 | 1100 | C |
| 5 | 0101 | 5 | 13 | 1101 | D |
| 6 | 0110 | 6 | 14 | 1110 | E |
| 7 | 0111 | 7 | 15 | 1111 | F |

- Binary advantages: simple arithmetic, easy chip design, two-level signals minimize errors
- Octal/Hex not directly understood by computers; used to shorten binary code for programmers
- Positional example: Decimal 1743 = 1×10³ + 7×10² + 4×10¹ + 3×10⁰ = 1000 + 700 + 40 + 3

**Worked Example 1: Decimal 25 → Binary (Division by 2)**

| Step | Division | Quotient | Remainder |
|------|----------|----------|-----------|
| 1 | 25 ÷ 2 | 12 | **1** |
| 2 | 12 ÷ 2 | 6 | **0** |
| 3 | 6 ÷ 2 | 3 | **0** |
| 4 | 3 ÷ 2 | 1 | **1** |
| 5 | 1 ÷ 2 | 0 | **1** |

Read remainders **bottom to top** → **(25)₁₀ = (11001)₂**
Verify: 1×16 + 1×8 + 0×4 + 0×2 + 1×1 = 16 + 8 + 1 = 25 ✓

**Worked Example 2: Decimal 58 → Binary**

| Step | Division | Quotient | Remainder |
|------|----------|----------|-----------|
| 1 | 58 ÷ 2 | 29 | **0** |
| 2 | 29 ÷ 2 | 14 | **1** |
| 3 | 14 ÷ 2 | 7 | **0** |
| 4 | 7 ÷ 2 | 3 | **1** |
| 5 | 3 ÷ 2 | 1 | **1** |
| 6 | 1 ÷ 2 | 0 | **1** |

Read remainders bottom to top → **(58)₁₀ = (111010)₂**
Verify: 32 + 16 + 8 + 0 + 2 + 0 = 58 ✓

**Worked Example 3: Decimal 13 → Binary (Sum of Weights Method)**

| Bit Position | 2³ | 2² | 2¹ | 2⁰ |
|--------------|----|----|----|----|
| Weight | 8 | 4 | 2 | 1 |
| Binary digit | 1 | 1 | 0 | 1 |

(13)₁₀ = 1×8 + 1×4 + 0×2 + 1×1 = **1101**₂

**Worked Example 4: Binary 11010110 → Hexadecimal**

Group binary digits into **4-bit nibbles from the right** (pad left with 0 if needed):

```
  1101  0110
   ↓     ↓
   D     6
```

(11010110)₂ = **(D6)₁₆

**Worked Example 5: Binary 11101001 → Hexadecimal**

```
  1110  1001
   ↓     ↓
   E     9
```

(11101001)₂ = **(E9)₁₆

**Worked Example 6: Binary 10110101 → Decimal**

| Bit | 2⁷ | 2⁶ | 2⁵ | 2⁴ | 2³ | 2² | 2¹ | 2⁰ |
|-----|----|----|----|----|----|----|----|----|
| Value | 1 | 0 | 1 | 1 | 0 | 1 | 0 | 1 |

= 128 + 0 + 32 + 16 + 0 + 4 + 0 + 1 = **(181)₁₀**

**Worked Example 7: Hex A3 → Binary → Decimal**

A = 1010, 3 = 0011 → (A3)₁₆ = (10100011)₂
= 128 + 32 + 0 + 0 + 0 + 2 + 1 = **(163)₁₀**

**Worked Example 8: Decimal 357 → Octal**

357 ÷ 8 = 44 R **5**; 44 ÷ 8 = 5 R **4**; 5 ÷ 8 = 0 R **5**
Read remainders bottom to top → **(357)₁₀ = (545)₈**
Verify: 5×64 + 4×8 + 5×1 = 320 + 32 + 5 = 357 ✓

**Worked Example 9: Octal 545 → Binary**

Each octal digit maps to 3 bits: 5=101, 4=100, 5=101 → **(101100101)₂

**Worked Example 10: Hex 2F → Decimal**

2×16 + 15×1 = 32 + 15 = **(47)₁₀

**Worked Example 11: Decimal 255 → Hex**

255 ÷ 16 = 15 R **15 (F)**; 15 ÷ 16 = 0 R **15 (F)** → **(255)₁₀ = (FF)₁₆

**Quick Conversion Reference**

| From | To | Method |
|------|----|--------|
| Decimal → Binary | — | Repeated division by 2; read remainders bottom-up |
| Binary → Decimal | — | Sum of (digit × 2^position) for each bit |
| Binary → Hex | — | Group into 4-bit nibbles from right; pad left with 0 |
| Hex → Binary | — | Each hex digit → 4-bit binary (e.g., F → 1111) |
| Decimal → Octal | — | Repeated division by 8; read remainders bottom-up |
| Octal → Binary | — | Each octal digit → 3-bit binary |

**For Exam**
Number systems used in computers include Binary (base-2, digits 0 and 1; bit, nibble, byte), Decimal (base-10), Octal (base-8, each digit = 3 bits), and Hexadecimal (base-16, digits 0–9 and A–F, each digit = 4 bits). Binary is the only language directly understood by computers because IC chips operate on two voltage states. Octal and hexadecimal provide compact representations of binary data for programmers.

**Diagram (refer SLM):** Fig. 1.2.1(a)(b) Binary system; Fig. 1.2.2(a)(b) Decimal; Fig. 1.2.3(a)(b) Octal; Fig. 1.2.4(a)(b) Hexadecimal; Fig. 1.2.5 Number System and Range.

#### 1.2.2 Digital Codes 🔥

**Theory**
When key 'A' is pressed, it is mapped to decimal code 65, then converted to binary for the computer. Digital coding uses binary digits to represent letters, characters, and symbols. Common codes include BCD (each decimal digit in 4 bits), Gray code (consecutive values differ by one bit), Excess-3 (add 3 to each decimal digit, express in 4-bit binary), and ASCII (7-bit character encoding). These codes bridge human-readable data and machine-level binary representation.

**Important Points**

| Code | Description | Example |
|------|-------------|---------|
| **BCD** | Binary-Coded Decimal; each decimal digit → 4 bits | (357)₁₀ = 0011 0101 0111; (123)₁₀ = 0001 0010 0011 |
| **Gray Code** | Consecutive numbers differ by only 1 bit; used in encoders, error detection | 0→000, 1→001, 2→011, 3→010, 4→110, 5→111, 6→101, 7→100 |
| **Excess-3** | Add 3 to each decimal digit, express in 4-bit binary; self-complementary | (23)₁₀: 2+3=5→0101, 3+3=6→0110 → **0101 0110** |
| **ASCII** | American Standard Code for Information Interchange; 7-bit; 128 standard codes | A=65, a=97; Standard ASCII (English) + Extended ASCII (special chars) |
| **EBCDIC** | 8-bit alphanumeric code by IBM; 256 symbols; used in mainframes | — |

**Digital Codes Comparison Table**

| Feature | BCD | Gray Code | Excess-3 | ASCII |
|---------|-----|-----------|----------|-------|
| **Full form** | Binary-Coded Decimal | Gray Code (Frank Gray) | Excess-3 Code | American Standard Code for Information Interchange |
| **Type** | Weighted code | Non-weighted code | Unweighted, self-complementary | 7-bit character encoding |
| **Rule** | Each decimal digit → 4 binary bits separately | Consecutive values differ by exactly 1 bit | Add 3 to each decimal digit, then 4-bit binary | Numeric code represents each character |
| **Bit length** | 4 bits per decimal digit | Variable (n bits for n values) | 4 bits per decimal digit | 7 bits (128 standard codes) |
| **Use** | Calculators, digital clocks, decimal arithmetic | Optical encoders, error detection in communication | Simplified BCD arithmetic operations | Letters, numerals, punctuation in English |
| **Example (digit 5)** | 0101 | 0111 (decimal 5 in 3-bit Gray) | 1000 (5+3=8 → 1000) | '5' = 53 (decimal) |
| **Example (letter A)** | Not used for letters | Not used for letters | Not used for letters | A = 65, a = 97 |
| **Limitation** | Wastes bits (1010–1111 unused per digit) | Not suitable for arithmetic directly | Extra step of adding 3 | Only 128 standard characters |

**Excess-3 Table (0–7)**

| Decimal | Binary | Excess-3 | Decimal | Binary | Excess-3 |
|---------|--------|----------|---------|--------|----------|
| 0 | 0000 | 0011 | 4 | 0100 | 0111 |
| 1 | 0001 | 0100 | 5 | 0101 | 1000 |
| 2 | 0010 | 0101 | 6 | 0110 | 1001 |
| 3 | 0011 | 0110 | 7 | 0111 | 1010 |

**Gray Code Table (0–7)**

| Decimal | Binary | Gray Code | Decimal | Binary | Gray Code |
|---------|--------|-----------|---------|--------|-----------|
| 0 | 000 | 000 | 4 | 100 | 110 |
| 1 | 001 | 001 | 5 | 101 | 111 |
| 2 | 010 | 011 | 6 | 110 | 101 |
| 3 | 011 | 010 | 7 | 111 | 100 |

**ASCII Quick Reference**

| Character | ASCII (Dec) | Binary (7-bit) | Character | ASCII (Dec) | Binary (7-bit) |
|-----------|-------------|----------------|-----------|-------------|----------------|
| 0 | 48 | 0110000 | A | 65 | 1000001 |
| 1 | 49 | 0110001 | B | 66 | 1000010 |
| 9 | 57 | 0111001 | Z | 90 | 1011010 |
| Space | 32 | 0100000 | a | 97 | 1100001 |

**Worked Example: BCD encoding of 357**
(357)₁₀ → 3=0011, 5=0101, 7=0111 → **0011 0101 0111**

**Worked Example: Excess-3 encoding of 23**
2+3=5→0101; 3+3=6→0110 → **0101 0110**

**Worked Example: ASCII for "Hi"**
H = 72 = 1001000; i = 105 = 1101001

**For Exam**
Digital codes represent characters and numbers in binary form. BCD encodes each decimal digit separately in 4 bits (e.g., 357 = 0011 0101 0111). Gray code ensures consecutive values differ by one bit, useful in encoders. Excess-3 adds 3 to each decimal digit before 4-bit binary encoding (23 → 0101 0110). ASCII uses 7-bit codes for characters (A=65, a=97). EBCDIC is IBM's 8-bit code with 256 symbols.

### Unit Recap (from SLM)
- Machine language (binary) is the only language directly understood by computers
- Number system = set of values to represent quantity; base/radix = number of unique digits
- Binary: base-2; bit, nibble (4 bits), byte (8 bits); MSB, LSB
- Decimal: base-10; Octal: base-8; Hexadecimal: base-16
- BCD: each decimal digit in 4 bits; Gray code: consecutive numbers differ by one bit
- Excess-3: add 3 to each digit, express in 4-bit binary
- ASCII: 7-bit character encoding; A=65, a=97


#### 1.4.3 Types of Computers 🔥

**Theory**
Computers are classified by size, power, and usage into seven categories. From smallest processing power (wearables, handheld) to largest (supercomputers), each type serves specific needs — portability for laptops, computing power for workstations, multi-user support for mainframes, and massive parallel processing for supercomputers used in weather forecasting and scientific research.

**Important Points**

| Type | Description | Use |
|------|-------------|-----|
| **Notebook/Laptop** | Battery/AC powered; fits briefcase; keyboard, touchpad, screen | Travel, libraries, meetings, aircraft |
| **Personal Computer (PC)** | General-purpose, non-portable; fits office desk; single user | Home, office workspace |
| **Workstation** | Powerful desktop; more computing power, storage, graphics than PC | Engineers, architects, professionals |
| **Mainframe** | Large, expensive; hundreds to thousands of simultaneous users | Organizations, banks; below supercomputer in hierarchy |
| **Supercomputer** | Fastest; huge storage and computational power; MIPS | Weather analysis, scientific/numerical problems; e.g., IBM Deep Blue |
| **Handheld (PDA)** | Small, held in hand; Tablet PC, PDA, Smartphone | Gaming, presentations, word processing |
| **Wearable** | Very small; worn on body; low processing power | Medicine: pacemakers, insulin meters |

**For Exam**
Computers by size and use include Notebook/Laptop (portable, battery-powered), Personal Computer (desktop, single user), Workstation (powerful desktop for professionals), Mainframe (supports hundreds/thousands of users), Supercomputer (fastest, MIPS, weather forecasting), Handheld/PDA (smartphone, tablet), and Wearable (pacemakers, insulin meters). IBM Deep Blue is an example of a supercomputer.

**Diagram (refer SLM):** Fig. 1.4.1 Different types of computers; Fig. 1.4.6 Notebook; Fig. 1.4.7 PC; Fig. 1.4.8 Workstation; Fig. 1.4.9 Mainframe; Fig. 1.4.10 Supercomputer; Fig. 1.4.11 Handheld; Fig. 1.4.12 Wearable.

### Unit Recap (from SLM)
- Early devices (Abacus, Napier's Bones, Pascaline) led to modern computers
- Charles Babbage = father of computers; Claude Shannon = binary system
- Characteristics: Automatic, Speed, Accuracy, Diligence, Versatility, Storage, No IQ, No Feeling
- By operating principle: Analog (continuous), Digital (digits/binary), Hybrid (both)
- By size/use: Notebook, PC, Workstation, Mainframe, Supercomputer, Handheld, Wearable
- MIPS = Millions of Instructions Per Second (supercomputers)


### Unit 1: Memory Representations and Hierarchy

#### 2.1.1 Computer Memory 🔥

**Theory**
Computer memory is the storage space where data and instructions are stored — temporarily or permanently. Memory is physically organized as cells (each storing 1 bit) made of semiconducting materials, with unique addresses for access. Memory is classified as volatile (contents erased when power off — RAM) or non-volatile (retains contents — ROM, secondary). The memory hierarchy — Registers → Cache → Main Memory → Secondary → Offline (tape) — balances speed, size, and cost, with faster/smaller/expensive storage at the top.

**Important Points**

| Topic | Details |
|-------|---------|
| **Structure** | Cells store 1 bit each; unique address per cell; bits grouped into memory words |
| **Units** | KB = 2¹⁰ = 1024 bytes; MB = 1024 KB; GB = 1024 MB; TB = 1024 GB; PB = 1024 TB |
| **Operations** | **Read** (fetch by address) and **Write** (store by address); **Access time** = time to read/write |
| **Primary Memory** | Directly accessed by CPU; RAM (volatile, read/write) + ROM (non-volatile); also called main/working memory |
| **SRAM vs DRAM** | SRAM: transistors only, no refresh, faster, expensive, used in cache; DRAM: transistor+capacitor, needs refresh, cheaper, used in main memory |
| **Secondary Memory** | Not directly accessed by CPU (needs interface); non-volatile, large, cheap; HDD, CD, DVD |
| **Cache Memory** | High-speed semiconductor between CPU and main memory; L1 (inside processor), L2, L3 (outside); hit/miss/penalty |
| **Memory Hierarchy** | Registers → Cache → Main → Secondary → Offline; top=volatile/fast/small/expensive; bottom=non-volatile/slow/large/cheap |

**SRAM vs DRAM**

| Feature | SRAM | DRAM |
|---------|------|------|
| Components | Transistors only | Transistors + capacitors |
| Refresh | Not required | Required periodically |
| Speed | Faster | Slower |
| Cost | Expensive | Cheaper |
| Density | Low | High |
| Use | Cache memory | Main memory |

**Cache Concepts**

- **Cache hit:** data found in cache; **Cache miss:** data not in cache
- **Miss penalty:** extra time to fetch data from main memory into cache
- **Hit ratio** = hits / (hits + misses) = no. of hits / total accesses

**Memory Hierarchy — Diagram Description (refer SLM Fig. 2.1.5)**

The memory hierarchy is a pyramid structure with the CPU at the top. Data flows between levels — when the CPU needs data, it searches from the fastest level downward until found, then copies data upward into faster levels for future access.

```
                    ┌─────────────┐
                    │     CPU     │
                    └──────┬──────┘
                           │
                    ┌──────▼──────┐
                    │  Registers  │  ← Fastest, smallest, most expensive
                    └──────┬──────┘
                           │
                    ┌──────▼──────┐
                    │  L1 Cache   │  ← Inside processor chip
                    └──────┬──────┘
                           │
                    ┌──────▼──────┐
                    │  L2 Cache   │  ← Outside processor
                    └──────┬──────┘
                           │
                    ┌──────▼──────┐
                    │  L3 Cache   │  ← Shared among CPU cores
                    └──────┬──────┘
                           │
                    ┌──────▼──────┐
                    │ Main Memory │  ← RAM (DRAM)
                    │    (RAM)    │
                    └──────┬──────┘
                           │
                    ┌──────▼──────┐
                    │  Secondary  │  ← HDD, SSD, Optical
                    │   Storage   │
                    └──────┬──────┘
                           │
                    ┌──────▼──────┐
                    │   Offline   │  ← Magnetic tape (backup)
                    │   Storage   │
                    └─────────────┘
```

**Memory Hierarchy — Access Time and Characteristics**

| Level | Location | Volatile? | Relative Speed | Typical Size | Cost/bit | Typical Access Time |
|-------|----------|-----------|----------------|--------------|----------|---------------------|
| **Registers** | Inside CPU | Yes | Fastest | Bytes (tens) | Highest | < 1 ns |
| **L1 Cache** | Inside processor chip | Yes | Very fast | 32–64 KB | Very high | ~1 ns |
| **L2 Cache** | On/near CPU die | Yes | Fast | 256 KB–1 MB | High | ~3–10 ns |
| **L3 Cache** | Outside CPU cores | Yes | Fast | 4–32 MB | High | ~10–20 ns |
| **Main Memory (RAM)** | Motherboard | Yes | Moderate | 4–64 GB | Moderate | ~50–100 ns |
| **SSD** | Internal/external | No | Faster than HDD | 256 GB–4 TB | Medium | ~10–100 μs |
| **HDD** | Internal/external | No | Slow | 500 GB–16 TB | Low | ~5–10 ms |
| **Optical (CD/DVD/BD)** | Removable drive | No | Slower | MB–GB | Very low | ~100 ms |
| **Magnetic Tape** | External backup | No | Slowest | TB+ | Lowest | Seconds (sequential) |

**Hierarchy Rules (from SLM)**

- **Top → Bottom:** speed decreases, storage size increases, cost per bit decreases
- **Bottom → Top:** access time decreases, cost per bit increases
- **Top three levels** (Registers, Cache, Main Memory) are **volatile**
- **Bottom two levels** (Secondary, Offline) are **non-volatile**
- College library analogy: study table = cache; department library = primary; central library = secondary

**For Exam**
Computer memory stores data and instructions in bit-level cells with unique addresses. Units: KB through PB (each × 1024). Primary memory (RAM volatile, ROM non-volatile) is directly accessed by CPU; secondary memory provides permanent bulk storage. Cache (L1/L2/L3) stores frequently used data between CPU and main memory. Memory hierarchy from Registers (fastest) to Offline tape (slowest) optimizes performance, capacity, and cost.

**Diagram (refer SLM):** Fig. 2.1.1 Different memories; Fig. 2.1.2 Structure of memory; Fig. 2.1.3 Memory cells analogy; Fig. 2.1.4 Cache Memory; Fig. 2.1.5 Memory Hierarchy.

### Unit Recap (from SLM)
- Memory cells store 1 bit; addressed by unique numbers
- Read and Write are main operations; access time = read/write duration
- Units: KB, MB, GB, TB, PB (each × 1024)
- Primary (RAM/ROM), Cache, Secondary — three memory types
- SRAM (cache) vs DRAM (main memory)
- Cache hit/miss/penalty; L1/L2/L3 cache levels
- Memory hierarchy: Registers → Cache → Main → Secondary → Offline

### Unit 2: Instruction Set and Instruction Cycle

#### 2.2.1 Instructions and Instruction Set 🔥

**Theory**
Instructions are the words of a computer's language — one step in a program for performing a specific task. A set of instructions forms a program; programs bundled together form software. The instruction set is the complete vocabulary of instructions a microprocessor supports (e.g., 8086 has ~117 basic instructions). Instruction Set Architecture (ISA) is the interface between hardware and software — the only way to interact with hardware. General instruction format has two fields: Opcode (operation to perform) and Address (operands).

**Important Points**

| Sample Instructions (8086) | Operation |
|---------------------------|-----------|
| ADD | Adding two numbers |
| COMPARE | Compare two numbers |
| IN | Input from device (keyboard) |
| LOAD | Load from RAM to register |
| OUT | Output to device (monitor) |
| STORE | Store from register to RAM |
| JUMP | Jump to designated address |

- Instruction format: **Opcode field** + **Address field** (e.g., ADD A, B — ADD=operator, A,B=operands)
- Address types: One-address, Two-address, Three-address instructions
- ISA = only way to interact with hardware

**For Exam**
Instructions are single steps in a program; instruction set is the complete group of instructions a microprocessor supports. ISA is the hardware-software interface. Instruction format contains Opcode field (operation) and Address field (operands). Example: ADD A, B adds operands A and B. Programs form software when bundled together.

#### 2.2.2 Instruction Cycle 🔥

**Theory**
A program in memory has a sequence of instructions executed through a cycle for each instruction. The instruction cycle has four phases: (1) Instruction Fetch — processor takes instruction from memory; (2) Instruction Decode — identifies operation and operands; (3) Operand Fetch — retrieves operand values from memory addresses; (4) Execution — performs the specified operation. For ADD A, B: fetch instruction, decode as addition with operands A and B, fetch values of A and B, execute A+B, store result.

**Instruction Cycle — Step-by-Step Explanation**

| Phase | Step | What Happens | Registers Involved |
|-------|------|--------------|-------------------|
| **1. Instruction Fetch** | 1a | CPU reads memory address stored in **PC** (Program Counter) | PC holds address of next instruction |
| | 1b | Instruction at that address is copied into **IR** (Instruction Register) | IR ← instruction from memory |
| | 1c | PC is incremented to point to the following instruction | PC = PC + 1 |
| **2. Instruction Decode** | 2a | **Control Unit (CU)** interprets the opcode field in IR | CU reads IR |
| | 2b | CU identifies the operation to perform (e.g., ADD, LOAD, JUMP) | — |
| | 2c | CU identifies operand locations (registers or memory addresses) | — |
| **3. Operand Fetch** | 3a | CPU retrieves operand values from memory using addresses in instruction | **MAR** ← memory address |
| | 3b | Data at that address is read into **MDR** (Memory Data Register) | MDR ← data from memory |
| | 3c | Operands loaded into appropriate registers for ALU use | GPR, Accumulator |
| **4. Execution** | 4a | **ALU** performs the operation specified by decoded instruction | Accumulator |
| | 4b | Result stored in destination (accumulator, register, or memory) | Result → Accumulator or MDR |
| | 4c | **Condition flags** updated if applicable (zero flag, carry flag) | Condition Code Register |

**Complete Worked Example: ADD A, B**

| Step | Phase | Action |
|------|-------|--------|
| 1 | Load program | Program containing ADD A, B is loaded into main memory |
| 2 | Instruction Fetch | PC points to ADD A,B; instruction fetched from memory into IR |
| 3 | Instruction Decode | CU identifies: Operation = **ADD**, Operands = **A** and **B** |
| 4 | Operand Fetch | Values of A and B fetched from memory addresses into registers |
| 5 | Execution | ALU computes A + B; result stored in Accumulator |
| 6 | Store | Result written back to memory location A (destination operand) |
| 7 | Repeat | PC points to next instruction; cycle repeats for entire program |

**Important Points**

- **Four phases:** Fetch → Decode → Operand Fetch → Execute
- Program must be loaded into main memory before execution begins
- PC (Program Counter) always holds address of the **next** instruction to fetch
- IR holds the instruction **currently being** decoded/executed
- Each instruction in the program goes through the complete cycle sequentially
- When not running, programs are stored in **secondary memory**

**For Exam**
The instruction cycle executes each program instruction in four phases: Instruction Fetch (CPU reads instruction from memory address in PC into IR, then increments PC), Instruction Decode (CU interprets opcode and identifies operands), Operand Fetch (values retrieved from memory via MAR/MDR into registers), and Execution (ALU performs operation, result stored). For ADD A, B: fetch instruction, decode as addition, fetch values of A and B, execute A+B, store result in A.

**Diagram (refer SLM):** Fig. 2.2.1 Instruction Cycle.

#### 2.2.3 RISC and CISC 🔥

**Theory**
RISC (Reduced Instruction Set Computer) uses a simple, limited instruction set with simple hardware; instructions like LOAD/STORE are independent; each instruction takes a single clock cycle; examples: PowerPC, SPARC. CISC (Complex Instruction Set Computer) uses complex instructions that can be larger than one word; reduces program instruction count but increases cycles per instruction; examples: VAX, Intel x86, AMD. RISC suits high-end applications (telecom, image/video processing); CISC suits low-end applications (home automation, security).

**Important Points**

| Feature | RISC | CISC |
|---------|------|------|
| Instruction set | Simple, limited | Complex, large |
| Decoding | Simple | Complex |
| Execution time | Short (single clock cycle) | Longer (multiple cycles) |
| Instruction format | Fixed | Variable |
| Memory interaction | Register-to-register (LOAD/STORE) | Memory-to-memory |
| Code length | Longer | Shorter (less RAM) |
| Examples | PowerPC, SPARC | VAX, Intel x86, AMD |
| Applications | High-end: telecom, image processing | Low-end: home automation |

**For Exam**
RISC uses simple instructions executed in single clock cycles with register-to-register operations (PowerPC, SPARC). CISC uses complex instructions reducing program size but requiring more cycles per instruction (Intel x86). RISC has simple decoding and fixed format; CISC has complex decoding and variable format. RISC suits high-performance applications; CISC reduces memory requirements with compact code.

### Unit Recap (from SLM)
- Instructions are words of computer language; programs form software
- Instruction set = all instructions a microprocessor supports
- Instruction format: Opcode field + Address field
- Instruction cycle: Fetch → Decode → Operand Fetch → Execute
- RISC: simple, fast, single cycle; CISC: complex, compact code
- ISA is the only way to interact with hardware

### Unit 3: Registers, Cache Memory and Virtual Memory

#### 2.3.1 CPU Registers 🔥

**Theory**
Registers are the fastest storage in the memory hierarchy — small temporary storage inside or near the CPU for fast data retrieval during instruction execution. They are classified by purpose into general types (Data, Address, Status/Flag registers) and specific registers (Accumulator, MAR, MDR, GPR, PC, IR, Condition Code). Registers are accessed at higher speed than conventional memory and are essential for CPU performance.

**Important Points**

| Register | Full Name | Function |
|----------|-----------|----------|
| **Data Register** | — | Holds data for an operation |
| **Address Register** | — | Holds address of data or instructions |
| **Status/Flag Register** | — | Indicates processor status or result of arithmetic operation |
| **Accumulator** | ACC | Stores intermediate results after ALU arithmetic/logical operations |
| **MAR** | Memory Address Register | Holds address of memory location to be accessed |
| **MDR** | Memory Data Register | Holds data to be read from or written to memory |
| **GPR** | General Purpose Register | R0, R1…Rn-1; temporary data during operations |
| **PC** | Program Counter | Contains address of next instruction to be executed |
| **IR** | Instruction Register | Stores instruction about to be executed (fetched from PC) |
| **Condition Code Register** | — | Contains 1-bit flags (0 or 1) indicating operation status (e.g., zero flag) |

- Registers = top of memory hierarchy; fastest storage mechanism
- Internal registers (inside processor) vs external registers (outside processor)

**For Exam**
CPU registers are the fastest temporary storage at the top of memory hierarchy. Key registers: MAR (memory address), MDR (memory data), Accumulator (ALU results), PC (next instruction address), IR (current instruction), GPR (temporary data), and Condition Code Register (1-bit flags). Registers enable fast data retrieval for instruction execution.

**Diagram (refer SLM):** Fig. 2.3.1 Memory hierarchy; Fig. 2.3.3 Registers in CPU.

#### 2.3.2 Cache Memory 🔥

**Theory**
Cache memory is very high-speed memory lying just below registers in the hierarchy, between the processor and main memory. Frequently used instructions and data are placed in cache for faster access. Three levels exist: L1 (primary, inside processor chip, smallest/fastest), L2 (secondary, outside processor, larger), L3 (shared among CPU cores in multi-core processors). Cache hit means data found in cache; cache miss requires fetching from main memory (miss penalty). Hit ratio = hits / (hits + misses) measures cache performance.

**Important Points**

- L1 = inside processor; L2/L3 = outside processor; L1 has lowest latency
- **Hit ratio** = hits / (hits + misses)
- Advantages: faster than main memory, less access time, stores frequently executed programs
- Disadvantages: limited capacity, high cost
- On miss: fetch from main memory → if not there, fetch from secondary → copy to main → copy to cache

**For Exam**
Cache memory is high-speed storage between CPU and main memory storing frequently used data. Three levels: L1 (inside processor, fastest), L2, L3 (outside, shared in multi-core). Cache hit = data in cache; cache miss = not found (miss penalty applies). Hit ratio = hits/(hits+misses) measures performance. Cache improves data retrieval efficiency despite limited capacity and high cost.

**Diagram (refer SLM):** Fig. 2.3.2 Cache memory; Fig. 2.3.4 Cache Memory.

#
#### 3.1.1 Software — System and Application 🔥

**Theory**

Software is a collection of computer programs, data, instructions, and documentation that enables a computer to perform specific tasks. An **instruction** is a step-by-step procedure; a **program** is a set of instructions; **hardware** is all physical parts; programs bundled together form **software**. The OS acts as the interface between user and hardware — the most important software on any computer. Software divides into **System Software** (manages hardware, provides platform) and **Application Software** (helps users perform specific tasks). Early systems used DOS (command-based); modern systems use GUI (graphical icons and mouse).

**Important Points**

| # | System Software | Application Software |
|---|-----------------|----------------------|
| 1 | Interface between apps and hardware | Designed per user requirements |
| 2 | Often low-level; also C, Python, Java | High-level languages |
| 3 | Operates computer hardware | Performs specific user tasks |
| 4 | Installed with OS | Installed per user need |
| 5 | Less/no user interaction | Full user interface |
| 6 | Runs independently; provides platform | Needs system software to run |
| 7 | OS, compilers, assemblers, debuggers, drivers | Word processors, browsers, media players |

- System software features: communicates directly with hardware, smaller size, complex, high speed, versatile
- **OS** = core system software; first layer loaded at startup; intermediary between user, apps, hardware
- **Device drivers** translate between OS and hardware (printers, graphics cards, network adapters)
- **Language processors:** assembler, compiler, interpreter — convert programming languages to machine code
- **Utility software:** compression tools, disk defragmenter, backup, antivirus
- Application: general purpose (word processor, spreadsheet, presentation, database, multimedia) or specific/customised (payroll, airline reservation, Tally, inventory/HRM)

**For Exam**

Software is a collection of programs, data, instructions, and documentation enabling computers to perform tasks. It divides into system software (manages hardware, provides platform — OS, device drivers, language processors, utilities) and application software (end-user programs — MS Office, browsers, payroll systems). System software communicates directly with hardware, is essential at startup, and runs independently; application software depends on it and provides user interfaces. General-purpose application software (word processor, spreadsheet) serves many users; specific-purpose software (Tally, airline reservation) is customised for one organisation. DOS was command-based; GUI allows interaction via graphical icons and mouse.


### Unit 2: Popular Operating Systems

#### 3.2.1 Operating System — Functions, DOS, Client-Server 🔥

**Theory**

An OS is a collection of software managing computer hardware and providing common services — the interface between user and hardware. Like a company manager, it coordinates all programs. **DOS** is disk-based, single-user, single-task, command-based OS. **Client-server** model: client requests services (like restaurant customer), server responds (like waiter). Open-source software has freely accessible source code; proprietary software is exclusively owned.

**Important Points**

| OS Function | Description |
|-------------|-------------|
| Process Management | Schedules and manages running programs/tasks |
| Memory Management | Allocates and tracks RAM usage |
| File System Management | Organises files and folders on storage |
| Device Management | Controls hardware via drivers |
| User Interface | Provides CLI (DOS) or GUI (Windows) interaction |
| Security & Access Control | Protects data; manages user permissions |
| Networking & Communication | Enables network and Internet connectivity |
| Error Handling & Logging | Records system errors for diagnosis |
| Virtualization/Multitasking | Runs multiple programs concurrently |
| Boot Process | Manages system startup sequence |

- **Device drivers** act as translators between OS and hardware (printers, graphics cards, network adapters)
- **Language processors** convert high-level code to machine code (assembler, compiler, interpreter)
- DOS: disk-based, single-user, single-task; user types commands; no graphical icons
- **Client** = requests services; **Server** = higher config, responds to requests
- Restaurant analogy: customer = client, waiter = server
- Every computer needs at least one OS; examples: Windows, Linux, Android, iOS

**For Exam**

An operating system manages hardware and provides common services as the user-hardware interface — like a company manager coordinating workers (applications). DOS is disk-based, single-user, single-task, command-based. In client-server computing, the client requests services and the server responds (restaurant customer/waiter analogy). OS handles process, memory, file, device management, security, networking, error handling, boot process, and time management. Device drivers translate for hardware; language processors convert code. Windows and Linux are common GUI OS; Android (Linux kernel) and iOS are dominant mobile OS.

#### 3.2.1.3 Types of Operating Systems 🔥

**Theory**

Operating systems are broadly classified into seven types based on how they manage users, tasks, processors, and networks. Each type suits different environments — from batch processing of similar jobs to real-time control systems and mobile devices.

**Important Points**

| OS Type | Key Feature | Examples |
|---------|-------------|----------|
| Batch OS | Similar jobs grouped as batches; offline input; no direct interaction | Punch card systems, payroll batch jobs |
| Multitasking/Time-sharing | Multiple terminal users simultaneously; quick response; reduces CPU idle time | UNIX, Multics |
| Multiprocessing | Two+ CPUs with OS copy each; coordinated multi-CPU operations | Windows NT, Windows 2000 |
| Real-Time OS | Immediate data processing; no delay permitted; hard/soft variants | Petroleum monitoring, military/space software |
| Distributed OS | Multiple systems on shared network; remote access, concurrency, fault tolerance | Cloud computing, Hadoop clusters |
| Network OS | Runs on servers; centralised user/data management; stable security | Windows Server 2003/2008, Novell NetWare, Mac OS X Server |
| Mobile OS | Smartphones, tablets, wearables; touch-optimised | Android, iOS, BlackBerry, watchOS |

- Real-time types: **Hard** (time constraint critical; delay = drastic consequences) | **Soft** (flexible timing)
- Real-time examples: petroleum temperature monitoring, military systems, space software
- Real-time advantages: maximum device utilisation, near error-free; limitation: complex algorithms
- Batch OS: jobs submitted via punch cards to operator; user does not interact during execution
- Time-sharing advantages: quick response, avoids software duplication, reduces CPU idle time
- Distributed advantages: effective resource sharing, concurrency, scalability, fault tolerance
- Network OS advantages: stable centralised servers, managed security, easy hardware upgradation
- Open-source: source code freely accessible (Linux); Proprietary: exclusively owned (Windows)

**For Exam**

Seven OS types with examples: **Batch** (punch card payroll jobs — no user interaction), **Multitasking/Time-sharing** (UNIX, Multics — multiple terminal users), **Multiprocessing** (Windows NT/2000 — multiple CPUs), **Real-Time** (petroleum/military/space — immediate response; hard/soft variants), **Distributed** (cloud/Hadoop — networked systems with fault tolerance), **Network OS** (Windows Server, Novell NetWare — server management), **Mobile OS** (Android, iOS — smartphones/tablets). Batch limitation: no interaction during job run. Distributed advantages: resource sharing, concurrency, scalability, fault tolerance.


#### 4.1.1 Computer Networks — Concepts, Need, and Working 🔥

**Theory**

A **computer network** connects computers and networking devices to share resources, data, and applications. Communication involves a **sender**, **transmission medium**, and **receiver** (Fig 4.1.1). **Guided medium** uses physical channels — copper cables, optical cables. **Unguided medium** is wireless — radio waves, microwaves, infrared. Networks enable file sharing, hardware sharing (printers), application sharing, and messaging without duplicating devices on each computer.

**Important Points**

- Network = connected devices sharing resources; connected device = **node** (PC, server, printer, switch)
- **Server/host** provides data, services, resources, programs to **clients** on request
- **Switch** connects all devices; sends, receives, forwards data across network ports
- **Shared printer workflow (4 steps):** PC-A sends print request → switch acknowledges → switch forwards to printer → printer prints document
- Family network analogy: members share resources; larger network connects to school, workplace, store
- Advantages: file-sharing (upload/download), hardware sharing (one printer for all), application sharing, messaging (WhatsApp, SMS)

**For Exam**

A computer network links computers and devices to share resources, data, and applications. Communication uses sender, medium, and receiver (Fig 4.1.1). Guided media (copper/optical cables) physically guide signals; unguided media (radio, microwaves, infrared) use wireless transmission. Without networks, each computer needs separate printers, scanners, and costly software. A basic network has nodes (PCs, server, printer) connected via a switch; the server provides services to clients on request. Shared printer workflow: PC sends request → switch acknowledges → switch forwards to printer → document prints.

#### 4.1.2 Types of Computer Networks 🔥

**Theory**

Networks are classified by geographical coverage into LAN, MAN, and WAN. Each serves different scales — from a single building to metropolitan areas to global connectivity without distance limitations.

**Important Points**

| Type | Coverage | Example |
|------|----------|---------|
| LAN | Small area: building/campus (few km) | Hospital departments, classroom |
| MAN | Metropolitan/city area | Cable TV network |
| WAN | Large geographical area; no distance limit | Inter-hospital national/global networks |

- LAN: hospital departments sharing info within one building/campus; most common type
- MAN: spans metropolitan/city area; example = cable TV connection network
- WAN: group of hospitals across country/world; no distance limitation; wireless global reach
- LAN limited to few kilometres; WAN has no geographic limit
- Classification based on coverage area, service type, and network requirements

**For Exam**

LAN covers a small geographical area like a hospital building or campus (few kilometres), enabling resource sharing within that site — the most frequently used network type. MAN spans a metropolitan/city area such as a cable TV connection network connecting an entire city. WAN covers large geographical areas with no distance limit — like a group of hospitals across countries sharing information wirelessly worldwide.

#### 4.1.3 Networking Devices 🔥

**Theory**

Networking devices (hardware/equipment) interconnect computers for data transfer and communication. They connect computers, printers, fax machines, and other devices. Five main types: Hub, Switch, Router, Repeater, and Bridge — each with distinct intelligence and function.

**Important Points**

| Device | Function | Key Trait |
|--------|----------|-----------|
| Hub | Connects multiple devices; broadcasts packets to ALL ports | Not secure; no intelligence |
| Switch | Forwards packets to designated port only | Intelligent; secure |
| Router | Connects different networks; chooses optimal route by destination | Links Network A to B |
| Repeater | Regenerates weakened signals | Extends transmission distance |
| Bridge | Divides LAN into segments; filters/forwards by address | Reduces traffic |

- Hub: data sent as packets to ALL connected ports (Fig 4.1.7 — nodes A–E); insecure
- Switch: receives data on designated port only; forwards to intended recipient (Fig 4.1.8)
- Router: checks destination address → chooses optimal route → forwards between networks (Fig 4.1.9)
- Repeater: strengthens weakened signal and retransmits (petrol pump analogy — Fig 4.1.10)
- Bridge: divides LAN into segments; checks address before forwarding (Fig 4.1.11)
- **Workstation:** dedicated business computer; high-resolution display, faster CPU, more RAM; multitasking; shares resources with clients/servers

**For Exam**

Hub connects multiple devices but broadcasts data packets to ALL ports — like a post office delivering to everyone at an address (insecure). Switch intelligently forwards packets only to the designated port — like registered post to one addressee (secure; replaces hubs today). Router connects two different networks, checks destination address, and chooses the optimal route (class teacher between two classes analogy). Repeater regenerates weakened signals over long distances (petrol pump refuelling analogy). Bridge divides a LAN into segments, filtering and forwarding by MAC address to reduce traffic.

#### 4.1.5 Network Topologies 🔥

**Theory**

**Topology** describes how computers are physically connected and the logical flow of information in a network. Six types: Bus, Ring, Star, Mesh, Tree, and Hybrid — each with distinct layout, fault tolerance, and cost. Physical topology = cable layout; logical topology = data flow path (may differ from physical).

**Important Points**

| Topology | Layout | Key Feature | Weakness |
|----------|--------|-------------|----------|
| Bus | Single backbone cable | Simple, cheap; all nodes share bus | Backbone failure stops entire network |
| Ring | Circular cable loop | Token controls access; orderly transmission | One break disrupts ring |
| Star | All nodes to central hub/switch | Easy to add/remove nodes; fault in one cable isolated | Hub failure disables all nodes |
| Mesh | Every node to every other | Fault tolerant; multiple paths; n(n-1)/2 edges | Expensive; complex wiring |
| Tree | Tree/branch (Bus + Star) | Scalable hierarchy; segmented traffic | Root/branch failure affects subtree |
| Hybrid | Mix of two+ topologies | Flexible for specific business needs | Complex to design and manage |

**Bus Topology** — single backbone; data travels both directions:
```
  [1]----[2]----[3]----[4]
       \______________/
         backbone bus
```

**Ring Topology** — token passes clockwise; node transmits only when holding token:
```
  [1]-->[2]
   ^     |
   |     v
  [4]<--[3]
```

**Star Topology** — all communication via central hub/switch:
```
      [HUB]
    /  |  |  \
  [1] [2][3] [4]
```

**Mesh Topology** — every node connected to every other; multiple paths:
```
  [1]=[2]    (= direct link)
  |\ /|
  [3]=[4]
```

**Tree Topology** — bus backbone with star branches via hubs:
```
       [H1]---[H2]
      / |       |\
    [1][2]    [3][4]
       |
     [H3]--[5]--[6]
```

**Hybrid Topology** — combines Bus + Star + Ring as needed:
```
  [Bus:1]--[Star Hub]--[2][3]
              |
         [Ring:4-5-6-7]
```

- Ring token system: data travels one direction; node transmits only when it holds the token
- Ring example: node 1→4 passes through 2, 3 sequentially; no start/end terminators in circle
- Mesh: if n=4 nodes, edges = 4×3/2 = 6; multiple alternate paths if one link fails
- Tree: node 1→6 path = node1 → hub1 → hub3 → node6; reduces traffic via segmentation
- Hybrid: node 1→2 uses star hub; node 1→6 uses bus then ring (needs token at node 6)
- Star weakness: central hub failure disables entire network; Bus weakness: backbone break stops all

**For Exam**

Topology is the physical connection and logical flow in a network. Bus uses one backbone cable — all nodes share it; cheap but backbone failure stops the network. Ring connects devices in a circle with no terminators; a token system ensures only the node holding the token can transmit (one direction). Star routes all traffic through a central hub/switch — easy to manage but hub failure is critical. Mesh connects every node to every other (n(n-1)/2 links) — fault tolerant but expensive. Tree combines bus backbone with star branches for scalable hierarchy. Hybrid mixes topologies (bus + star + ring) for flexible business needs.

#### 4.1.6 Network Operating Systems (NOS) ⭐

**Theory**

**NOS** coordinates communication of multiple computers across a network (unlike single-computer OS). Two major types: **Peer-to-Peer** (equal computers share resources, no central file server) and **Client/Server** (dedicated file servers with centralised security and management).

**Important Points**

| Type | Features | Suitability |
|------|----------|-------------|
| Peer-to-Peer | No file server; all computers equal; share files/resources | Small-medium LANs |
| Client/Server | Dedicated file server(s); centralised security; multi-user access | Larger organisations |

- P2P: share resources/files; access files on other computers; no central file server or centralised management
- P2P: all computers equal with same capabilities; designed for small-medium LANs
- Client/Server: centralise functions; one or more dedicated file servers with security
- Client/Server: integrate all devices; share resources with multiple users regardless of location
- NOS = OS for networks; coordinates multiple computers (unlike single-computer Windows/Linux)

**For Exam**

Network Operating System (NOS) coordinates multiple computers across a network — unlike Windows/Linux on a single PC. Peer-to-Peer NOS lets equal computers share files and resources without a central file server or centralised management, suitable for small-medium LANs. Client/Server NOS uses dedicated file server(s) providing centralised security, resource management, and multi-user access regardless of user location. P2P: all nodes equal; Client/Server: server has higher configuration and responds to client requests.

### Unit Recap (from SLM)
- Communication transfers information; medium may be **guided** (cables) or **unguided** (wireless)
- **Computer network** connects devices to share resources, data, applications
- **Server** provides data/services; **node** = any connected device; **switch** forwards data
- **LAN** = building/campus; **MAN** = city; **WAN** = no geographic limit
- **Hub** = broadcast (no intelligence); **Switch** = intelligent forwarding
- **Router** connects networks; **Repeater** regenerates signals; **Bridge** divides segments
- **Topology** = physical connection and logical flow; six types with distinct ASCII layouts
- **NOS:** Peer-to-Peer (no file server) vs Client/Server (dedicated file server)


#### 6.1.1 Applications of IT

**Theory**

**Information Technology (IT)** includes everything associated with computer technology — networking, hardware, software, the Internet, and the people who use them. IT is a wide discipline dealing with **processing, management, transfer, storage, protection, and retrieval** of information. Key associated terms: hardware, software, database, communication, server, network, Internet, applications. Major IT applications: business, banking, education, medical field, science, and mobile application development. Most organisations maintain IT departments. IT enables online advertising through Facebook, WhatsApp, and Twitter — saving time and money compared to offline media.

| IT Term | Definition |
|---------|-----------|
| **Hardware** | Physical parts: keyboard, mouse, monitor, speakers |
| **Software** | Programs that tell the computer how to work |
| **Database** | Organised collection of information for easy access/update |
| **Communication** | Transfer of information between computers (email, WhatsApp) |
| **Server** | Computer providing data, files, programs to other computers |
| **Network** | Collection of connected computers sharing resources |
| **Internet** | Global network of millions of computers worldwide |
| **Applications** | Practical implementation of IT in various fields |

**Important Points**

- IT = processing, management, transfer, storage, protection, retrieval of information
- Hardware = physical parts; Software = programs; Database = organised data
- Server provides data; Network connects computers; Internet = global network
- Applications: business, banking, education, medical, mobile apps
- IT enables online advertising via social media (saves time and money)
- Organisations have dedicated IT departments
- Communication transfers information via email, WhatsApp, etc.
- Database helps organise, access, manage, and update data easily

**For Exam**

Information Technology encompasses computer technology including networking, hardware, software, and the Internet. It deals with processing, management, transfer, storage, protection, and retrieval of information. Associated terms include hardware (physical parts), software (programs), database (organised data), server (provides data to other computers), network (connected computers sharing resources), and Internet (global network). Major applications span business, banking, education, healthcare, science, and mobile development. IT has become integral to modern organisational operations. Online advertising via social media saves time and money compared to offline newspaper/radio/TV ads.


### Unit 3: Computer Security and Malware

#### 6.3.1 Computer Security and Threats 🔥

**Theory**

**Computer Security** protects data and computer systems from harm, theft, and unauthorized use. Four major **threats**: (1) **Theft of data** — stealing secret/sensitive data from organisations; (2) **Computer Vandalism** — extracting passwords, erasing hard disk via malicious programs; (3) **Fraud** — unauthorized fund/data transfers; (4) **Invasion of privacy** — illegal access to personal/financial/medical databases. Countermeasures: security software (firewall, antivirus, antispyware), strong passwords, data backup on separate media, encryption. Six security measures: firewall, human aspects, data backup, cryptography, antivirus, anti-spyware.

| Security Measure | Description | Example |
|-----------------|-------------|---------|
| **Firewall** | Hardware/software filtering network traffic per security policy | Blocks prohibited inbound/outbound communications |
| **Human Aspects** | Protecting against unwanted user/intruder actions | Hardest task; training users against social engineering |
| **Data Backup** | File duplication for emergency recovery | WhatsApp backup; daily/weekly backup to separate server |
| **Cryptography** | Hides data by converting to coded representation | Encrypt "attack" as "@2&7?+"; decrypt with secret key |
| **Antivirus** | Identifies and removes viruses from memory/storage/email | Kaspersky, K7, Avira scan boot/OS modifications |
| **Anti-Spyware** | Finds and removes spyware secretly collecting data | Spybot Search and Destroy, Ad-aware |

**Important Points**

- Computer security = protection from harm, theft, unauthorized use
- Four threats: data theft, vandalism, fraud, privacy invasion
- Firewall filters network traffic per security policy
- Cryptography: encrypt/decrypt with keys
- Data backup = file duplication for recovery
- Antivirus identifies and removes viruses
- Intruder enters system without permission (e.g. hacker)
- WhatsApp data backup saves data on servers for recovery

**For Exam**

Computer security is the protection of data and computer systems from harm, theft, and unauthorized use. Four major threats are theft of data (stealing sensitive organisational data), computer vandalism (extracting passwords or erasing hard disk), fraud (unauthorized fund transfers), and invasion of privacy (illegal access to personal/financial/medical databases). Six security measures are firewall (filters network traffic), human aspects (user/intruder protection), data backup (file duplication for recovery), cryptography (encryption/decryption with keys), antivirus (removes viruses), and anti-spyware (removes Spybot). Strong passwords and encryption protect against unauthorized access.

#### 6.3.2 CIA Triad — Confidentiality, Integrity, Availability 🔥

**Theory**

Three elements of computer security: **Confidentiality** — concealment of information; only authorized persons access it (encrypted email with secret key; "Hello!" → encrypted as `f7#E+`). **Integrity** — trustworthiness of data; prevents unauthorized changes; sub-elements: data integrity (content) and authentication (originality); hashing converts data to unique text strings. **Availability** — ability to access data when needed by authorized users at the right time; server attacks cause unavailability. Together these form the **CIA triad** — the foundation of cybersecurity policy.

| CIA Element | Definition | Mechanism | Example |
|------------|-----------|-----------|---------|
| **Confidentiality** | Conceal information from unauthorized access | Encryption with secret key | Encrypted email readable only with key |
| **Integrity** | Data trustworthiness; prevent tampering | Hashing (# function) | Rs 500 payment protected from change to Rs 5000 |
| **Availability** | Authorized access when needed | Server uptime, backup systems | Bank server accessible for loan repayment |

**Important Points**

- Confidentiality = information secrecy; encryption with keys
- Integrity = data trustworthiness; prevents tampering
- Integrity sub-elements: data integrity + authentication
- Hashing converts data to unique string (# function)
- Availability = access when needed by authorized users
- CIA triad = Confidentiality, Integrity, Availability
- Example: Rs 500 payment changed to Rs 5000 = integrity loss
- Server attack preventing loan payment = availability loss

**For Exam**

The three elements of computer security are Confidentiality (concealing information so only authorized users access it, using encryption — e.g. "Hello!" encrypted as `f7#E+` with secret key), Integrity (maintaining data trustworthiness and preventing unauthorized changes like payment amount tampering, using hashing for authentication), and Availability (ensuring authorized users can access data when needed — server attacks cause unavailability). Together they form the CIA triad fundamental to cybersecurity. Computer security aims to prevent disruption of information and services.

#### 6.3.3 Security Terminology and Malware 🔥

**Theory**

Key terminologies: **Unauthorized access** — accessing server/data without owner knowledge. **Hacker** — exploits systems for money, cause, or fun. **Threat** — action/event compromising security. **Vulnerability** — flaw allowing attacker manipulation. **Attack** — assault violating security. **Social Engineering** — psychological manipulation to steal data. **Malware** — collective name for viruses, ransomware, worms, Trojans, adware, spyware; delivered via links/files over Internet requiring user click. **Spybot/Ad-aware** remove spyware; **Kaspersky, K7, Avira** are antivirus examples.

| Malware Type | Behaviour | Delivery Method | Key Damage |
|-------------|-----------|----------------|------------|
| **Virus** | Inserts into standalone program; spreads on execution | Email attachment, file download | Corrupts files; steals passwords |
| **Worm** | Self-replicating standalone software | Network, email without user action | Spreads automatically computer-to-computer |
| **Trojan** | Disguised as legitimate software | Tricked user installation | Takes control of system after install |
| **Ransomware** | Encrypts hard drive files | Link or file over Internet | Demands payment for decryption key |
| **Adware** | Forces browser redirect to advertisements | Bundled with free downloads | Downloads further malicious software |
| **Spyware** | Secretly collects sensitive user data | Installed without user knowledge | Sends data to external third parties |

| Term | Definition |
|------|-----------|
| **Unauthorized access** | Accessing server/website/data without owner's knowledge |
| **Hacker** | Person exploiting computer system for money, cause, or fun |
| **Threat** | Action or event that might compromise computer security |
| **Vulnerability** | Flaw/weakness in system allowing attacker manipulation |
| **Attack** | Assault on computer system security violating policies |
| **Social Engineering** | Stealing data via psychological manipulation, not hacking |

**Important Points**

- Six security measures: firewall, human aspects, backup, cryptography, antivirus, antispyware
- Malware = malicious software collective term
- Virus attaches to programs; worm self-replicates independently
- Trojan disguises as legitimate software
- Ransomware encrypts and demands payment
- Spyware/Adware steal data or force ad redirects
- Social engineering uses psychological tricks, not technical hacks
- Malware delivered as link or file; user must click to execute

**For Exam**

Computer security terminologies include unauthorized access (accessing data without owner knowledge), hacker (exploits systems for money or fun), threat (action compromising security), vulnerability (system flaw allowing manipulation), attack (assault on security), and social engineering (psychological manipulation to steal data). Malware is malicious software including viruses (attach to programs, spread on execution), worms (self-replicating standalone), Trojans (disguised as legitimate software), ransomware (encrypts files demanding payment), adware (forces browser ad redirects), and spyware (secret data collection). Malware is delivered via Internet links or files requiring user click to execute.

#### 6.3.4 Types of Computer Viruses 🔥

**Theory**

A **computer virus** attaches to program files, stays inactive until execution, then spreads across networks corrupting files, stealing passwords, and damaging systems. Spreads via email attachments, downloads, social media links. General signs: pop-ups, blue screen, homepage changes, bulk emails, crashes, missing files, slow performance, unknown startup programs, password changes, disabled security software. Like coronavirus spreading person-to-person, a computer virus infects one machine then spreads across the network.

**Important Points**

- Virus spreads on execution of infected program/file
- Signs: pop-ups, crashes, slow performance, missing files
- Boot sector virus infects boot sector via infected USB
- Polymorphic virus changes code to evade antivirus
- Multipartite attacks boot sector AND executable files
- Macro virus written in Word/Excel macro language
- Virus stays dormant until infected program is executed
- Spreads via email attachments and social media scam links

**General Virus Infection Signs:**

| Sign | Description |
|------|-------------|
| Repeated pop-up windows | Unexpected pop-ups appear frequently |
| Blue screen errors | System crashes with blue error screen |
| Homepage changes | Browser homepage altered without permission |
| Bulk emails sent | Emails sent from your account to contacts without your action |
| Repeated system crashes | Computer freezes or crashes frequently |
| Missing files | Files disappear from folders |
| Slow performance | Unusual slowness in normal operations |
| Unknown startup programs | Unfamiliar programs launch at boot |
| Password changes | Passwords changed without your knowledge |
| Disabled security software | Antivirus or firewall turned off by virus |

**For Exam**

Computer viruses attach to programs and spread on execution, causing file corruption, password theft, spam emails, and system damage via email attachments, Internet downloads, and social media links. Eight types exist: boot sector (boot-time infection via USB), web scripting (browser/webpage exploit), browser hijacker (modifies browser settings/redirects), resident (stays in memory after program closes), direct action (activates on .exe/.com execution), polymorphic (changes code each execution to evade antivirus), multipartite (attacks boot sector AND files — most dangerous), and macro virus (embedded in Word/Excel documents, runs on open). General signs include pop-ups, blue screen, homepage changes, bulk emails, crashes, missing files, slow performance, and disabled security software.

| Virus Type | Characteristic | Target / Behaviour | Symptoms / Signs |
|------------|---------------|--------------------|-----------------|
| **Boot Sector** | Copies code to boot sector of disk | Activates on startup; spreads via infected USB | System fails to boot; damage during startup from pen drive |
| **Web Scripting** | Explots web browser/page code | Infects when visiting affected webpage | Browser malfunctions after visiting infected site |
| **Browser Hijacker** | Modifies browser settings without permission | Redirects to unwanted sites; replaces homepage/search | Unwanted ads; redirects to money-making scam sites |
| **Resident** | Stays in memory after program closes | Continues running after software terminated | Damage persists even after uninstalling infected program |
| **Direct Action** | Activates only when infected file executes | Attaches to .exe and .com files | Files become inaccessible; no performance delay |
| **Polymorphic** | Changes its code each execution | Evades traditional antivirus detection | Antivirus fails to detect; virus reappears after scan |
| **Multipartite** | Attacks boot sector AND program files | Most dangerous; contaminates multiple times | Combined boot failure and file corruption simultaneously |
| **Macro** | Written in macro language (Word/Excel) | Embedded in documents; runs on document open | Infection spreads when opening Word/Excel attachments |

#### 6.3.5 Antivirus Software 🔥

**Theory**

**Antivirus** is software designed to prevent, search, detect, and remove malicious software. Essential because hackers release new viruses daily; unprotected computers get infected on Internet connection. Functions: scan files/directories/external devices, schedule automatic scans, remove detected malware, show computer health, parental controls, act as firewall, warn about dangerous websites, protect online accounts. Scans programs attempting to modify boot program, OS, or other protected programs.

**Important Points**

- Antivirus: prevent, search, detect, remove malware
- Scans files, directories, external devices
- Scheduled automatic scans
- Examples: Kaspersky, K7, Avira
- Anti-spyware (Spybot, Ad-aware) removes spyware
- New viruses daily require updated antivirus
- Warns about dangerous websites and links
- Can act as firewall and provide parental controls

**For Exam**

Antivirus software prevents, searches, detects, and removes malicious software from files and computer systems. It scans programs attempting to modify boot program, operating system, or other protected programs, schedules automatic scans, removes detected threats, monitors computer health, provides parental controls, acts as firewall, and warns about dangerous websites. Examples include Kaspersky, K7, and Avira. Anti-spyware programs like Spybot Search and Destroy and Ad-aware remove spyware secretly collecting user data. Updated antivirus is essential as hackers release new viruses daily; unprotected computers get infected immediately on Internet connection.

| Antivirus Function | Description |
|-------------------|-------------|
| Scan files/directories | Checks files, folders, external devices for malware |
| Scheduled automatic scans | Regular scans without manual initiation |
| Remove detected malware | Deletes or quarantines malicious programs |
| Monitor computer health | Shows overall security status of system |
| Parental controls | Restricts children's online activities |
| Warn dangerous websites | Alerts before visiting harmful links |
| Protect online accounts | Guards credentials and sensitive login data |

### Unit Recap — Unit 3

- Six security measures: firewall, human aspects, backup, cryptography, antivirus, antispyware
- Four threats: data theft, vandalism, fraud, privacy invasion
- CIA triad: Confidentiality, Integrity, Availability
- Malware types: virus, worm, Trojan, ransomware, adware, spyware
- Eight virus types: boot sector, web scripting, browser hijacker, resident, direct action, polymorphic, multipartite, macro
- Antivirus prevents, detects, and removes malware









### Block 6 Quick Reference — Key Terms Summary

| Topic | Key Terms / Facts |
|-------|------------------|
| **IT Definition** | Processing, management, transfer, storage, protection, retrieval of information |
| **Banking** | ECS (bulk), MICR (9-digit cheque code), NEFT (batch), RTGS (real-time/fastest), CBS (any-branch), ATM |
| **HIT / Medical IT** | MPM (practice management), EHR/EMR (digital records), RPM (remote sensors) |
| **Mobile Apps** | Native (platform-specific), HTML5 (cross-platform), Hybrid (native + HTML5) |
| **Bioinformatics** | IT + biology; Paulien Hogeweg 1979; databases + algorithms + analysis |
| **Security Measures** | Firewall, human aspects, backup, cryptography, antivirus, anti-spyware |
| **CIA Triad** | Confidentiality (encryption), Integrity (hashing), Availability (access when needed) |
| **Malware Types** | Virus, Worm, Trojan, Ransomware, Adware, Spyware |
| **8 Virus Types** | Boot sector, Web scripting, Browser hijacker, Resident, Direct action, Polymorphic, Multipartite, Macro |
| **VR Types** | Fully-Immersive, Semi-Immersive, Non-Immersive |
| **AR Types** | Marker Based, Superimposed, Location Based, Projection Based |
| **AI Types** | Narrow/Weak (Alexa), General/Strong (not yet), Super (hypothetical) |
| **AI Coined By** | John McCarthy, 1956 |
| **Smart Technology** | IoT devices, Smart Connected, Smart Devices |
| **IoT Components** | Sensors → Gateway → Server → Mobile/Laptop |
| **IoT Workflow** | Collect → Transport → Process → Trigger → Notify |
| **Quantum Computing** | Qubits; Silq language; emerged 1980s |
| **Nanotechnology** | 1–100 nm; STM/AFM microscopes |
| **Cloud Computing** | AWS; on-demand servers/storage over Internet |

---


## Quick Reference — Exam Essentials

| Topic | Must-Know |
|-------|-----------|
| Computer functions 🔥 | Input, Processing, Output, Storage |
| Hardware/Software/Firmware/Liveware 🔥 | Physical parts / Programs / ROM (BIOS) / Users |
| Von-Neumann 🔥 | Stored program; CU, ALU, memory, I/O |
| Number systems 🔥 | Binary, Decimal, Octal, Hex; BCD, Gray, Excess-3, ASCII |
| Memory hierarchy 🔥 | Registers → Cache → RAM → Secondary |
| Instruction cycle 🔥 | Fetch → Decode → Execute → Store |
| RISC vs CISC 🔥 | Simple/fast vs Complex/compact |
| Boot process 🔥 | POST → Boot loader → OS (warm vs cold boot) |
| Translators 🔥 | Compiler, Interpreter, Assembler |
| LAN/MAN/WAN 🔥 | Building / City / Worldwide |
| Topologies 🔥 | Bus, Ring, Star, Mesh, Tree, Hybrid |
| Email 🔥 | SMTP send; POP3/IMAP receive |
| HTML skeleton 🔥 | `<!DOCTYPE html><html><head><body>` |
| Banking IT | ECS, MICR, NEFT, RTGS, CBS, ATM |
| Security (CIA) 🔥 | Confidentiality, Integrity, Availability |
| Emerging tech 🔥 | VR, AR, AI, IoT, Quantum |

---



