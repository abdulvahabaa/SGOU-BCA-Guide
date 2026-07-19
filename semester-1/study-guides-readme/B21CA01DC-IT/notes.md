# Introduction to Information Technology — Study Notes

**Course Code:** B21CA01DC | **Semester:** I | **Programme:** BCA | **University:** Sreenarayanaguru Open University (SGOU)  
**Subject:** Introduction to Information Technology | **Coverage:** Blocks 1–6, 24 Units (Theory Only)  
**Source:** Self Learning Material (SLM) — SGOU BCA Semester I

---

### About These Notes

**Prepared by:** Abdul Vahab A A  
**Website:** https://abdulvahabaa.in

These notes were created for my personal study and revision. I am sharing them here because someone else might find them useful too.

**Wishing you all success** in your semester exams and IT learning journey. Stay disciplined, revise smartly, and keep confidence in your effort.

**Duaon mein Yaad Rakhna.**

---

## Index

Block 1: Computer Fundamentals — Hardware, number systems, I/O devices, computer types  
Block 2: Instructions, Memory and Storage — Memory hierarchy, instruction cycle, registers, secondary storage  
Block 3: Software — Boot process, OS, system software, application software  
Block 4: Networks and Internet — LAN/MAN/WAN, topologies, WWW, connectivity, email  
Block 5: Hypertext Markup Language — HTML tags, lists, tables, multimedia, linking  
Block 6: Trends in Information Technology — IT applications, security, VR/AR/AI/IoT  

*(Detailed subsection numbers match SGOU SLM — see each unit heading in the notes.)*

### Study Priority Markers

Use these while revising — matched to [Important Topics BCA Sem 1](../important-topics.md):

| Marker | Meaning |
|--------|---------|
| 🔥 | **Must revise** — asked in exams or in Exam Essentials |
| ⭐ | **Also important** — asked in past papers (revise after 🔥 topics) |
| No marker | Read once; lower exam frequency |

### Where to Focus — Quick Map

| Block | 🔥 Focus Sections | Why |
|-------|-------------------|-----|
| **Block 1** | 1.1.1, 1.1.2, 1.1.4, 1.1.5, 1.2.1, 1.2.2, 1.4.2, 1.4.3 | Computer basics, Von-Neumann, number systems, Gray/ASCII, computer types |
| **Block 2** | 2.1.1, 2.2.1–2.2.3, 2.3.1–2.3.3 | Memory hierarchy, instruction cycle, registers, RISC/CISC, cache, virtual memory |
| **Block 3** | 3.1.1, 3.1.3, 3.1.5, 3.2.1, 3.2.1.3, 3.2.1.4, 3.3.1, 3.3.2, 3.4.2 | System vs app software, boot/POST, OS types, translators, virus |
| **Block 4** | 4.1.1–4.1.3, 4.1.5, 4.2.2, 4.2.5, 4.2.7, 4.4.1 | LAN/MAN/WAN, devices, topologies, URL, search engines, email |
| **Block 5** | **All units** (5.1–5.4) | HTML — heavily asked every year |
| **Block 6** | 6.3.1–6.3.5, 6.4.1–6.4.3, 6.4.5 | Security, CIA, malware, VR/AR, AI, IoT |

**Revision order:** Block 5 (HTML) → Block 3 (OS/Software) → Block 4 (Networks) → Block 2 (Memory/CPU) → Block 1 → Block 6


---

## Block 1: Computer Fundamentals

### Unit 1: Basic Hardware Concepts

#### 1.1.1 Functions of a Computer 🔥

**Theory**
A digital computer is an electronic device that accepts user input, processes it, and generates the desired output. Like a juicer that takes fruit as input, processes it when the button is pressed, and produces juice as output, a computer transforms raw data into meaningful results through systematic processing. A computer performs four essential functions: accepting data (Input), performing operations on data as per instructions (Processing), providing the result to the user (Output), and retaining data for future use (Storage).

**Important Points**

- Four functions: **Input, Processing, Output, Storage**
- Input = data entered via keyboard, mouse, scanner, microphone, etc.
- Processing = operations performed on data according to program instructions
- Output = result displayed via monitor, printer, speakers, etc.
- Storage = saving processed data on memory devices (CD, USB, HDD, etc.)
- Alan Turing is considered the father of modern digital computers

**For Exam**
A digital computer is an electronic device that accepts input, processes it, and produces output. Its four functions are: (1) Input — accepting data through devices like keyboard and mouse; (2) Processing — performing operations on data per instructions; (3) Output — delivering results via monitor or printer; (4) Storage — saving data for future use. Computers require both hardware and software to function properly.

#### 1.1.2 Basic Concepts 🔥

**Theory**
When dealing with computers, four key terminologies appear frequently: Hardware, Software, Firmware, and Liveware. Together they describe the complete computer ecosystem — physical components, programs, embedded essential programs, and the human users who operate the system. A computer without software is like a book with blank pages; firmware ensures essential startup programs run from ROM; liveware represents the human element that gives computers their purpose.

**Important Points**

| Concept | Definition | Example |
|---------|------------|---------|
| **Hardware** | Physical, tangible parts that can be seen and touched | Keyboard, mouse, processor, printer |
| **Software** | Set of programs bundled together; program = step-by-step instructions for a task | Windows, Linux, application programs |
| **Firmware** | Essential programs stored in separate memory; user cannot modify or delete | BIOS (in ROM) — runs POST at startup |
| **Liveware** | Human users who operate computers in daily activities | Students, professionals, operators |

- Storybook analogy: cover/pages/ink = hardware; words/story = software
- POST (Power-on Self Test) checks hardware at startup using BIOS firmware

**For Exam**
Basic concepts of a computer system include Hardware (physical components like keyboard and processor), Software (set of programs that tell the computer what to do), Firmware (essential unmodifiable programs stored in ROM such as BIOS that runs POST at startup), and Liveware (human users). Hardware and software together make a computer useful, just as a book needs both physical pages and written content.

**Diagram (refer SLM):** Fig. 1.1.1 Computer System — keyboard, mouse, system unit, monitor, speaker, microphone.

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

#### 1.1.5 Hardware Fundamentals 🔥

**Theory**
The major hardware components of a computer are the CPU (Processor), Motherboard, Memory, SMPS, Hard disk drive, Optical storage, Solid State Drive, and Registers. The processor is the most crucial component controlling all computer activities. Memory is classified into primary (RAM, ROM — directly accessed by CPU) and secondary (HDD, SSD, optical — permanent bulk storage). SMPS acts as the power supply unit, like the heart pumping power to all components.

**Important Points**

| Component | Description |
|-----------|-------------|
| **Processor (CPU)** | Most crucial hardware; controls all activities; examples: Intel Core i7/i5, AMD Ryzen, Snapdragon |
| **Motherboard** | Printed circuit board (PCB); backbone connecting all devices |
| **RAM** | Volatile primary memory; read/write; contents lost when power off; reloaded from secondary at boot |
| **ROM** | Non-volatile primary memory; stores BIOS; types: PROM, EPROM (UV erase), EEPROM (electrical erase) |
| **Secondary Memory** | Non-volatile permanent storage — HDD, SSD, CD, DVD, USB |
| **Registers** | Small high-speed storage inside CPU; general-purpose and special-purpose |
| **SMPS** | Switched Mode Power Supply; PSU; better efficiency than linear supplies |

- Memory address = unique number identifying each memory location (like house number)
- SSD uses NAND flash; faster, shock-resistant, lower power than HDD
- Processor and CPU terms are used interchangeably

**For Exam**
Key hardware components include the Processor (CPU — controls all computer activities), Motherboard (backbone PCB connecting all devices), Memory (Primary: RAM volatile read/write, ROM non-volatile with BIOS; Secondary: HDD, SSD, optical for permanent storage), Registers (fast temporary CPU storage), and SMPS (power supply unit). ROM types include PROM (non-erasable), EPROM (UV erasable), and EEPROM (electrically erasable).

**Diagram (refer SLM):** Fig. 1.1.3 Processors; Fig. 1.1.4 Motherboard; Fig. 1.1.5 RAM; Fig. 1.1.6 ROM; Fig. 1.1.7 HDD; Fig. 1.1.8 DVD Drive; Fig. 1.1.9 SMPS.

### Unit Recap (from SLM)
- Computer receives data, processes it, and outputs the intended result
- Hardware = visible, touchable mechanical and electronic components
- Software = programs, OS, and data stored in memory/storage media
- Four essential components: input devices, output devices, memory, and CPU
- Input unit receives input; CPU processes (CU controls, ALU computes); memory stores during processing; output unit delivers results
- Von-Neumann architecture: ALU, Control Unit, Memory Unit, I/O — stored program concept
- Primary memory: RAM (volatile) and ROM (non-volatile); Secondary: HDD, SSD, optical
- Key hardware: Processor, Motherboard, Memory, SMPS, HDD, SSD, DVD drive, Registers

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

### Unit 3: Input/Output Devices

#### 1.3.1 Input Devices ⭐

**Theory**
Input/output devices allow the computer to interact with the outside world. Input devices accept data and instructions from the user and convert them into a form the computer can process. Without I/O devices, a computer would be a "dumb terminal" with no external communication. Common input devices include keyboard, mouse, touchpad, scanner, and barcode reader — each designed for specific data entry needs.

**Important Points**

| Device | Description |
|--------|-------------|
| **Keyboard** | Most common input device; QWERTY layout; 101-key standard; primary device for data/instructions |
| **Mouse** | Pointing device; controls cursor; point, drag, drop; types: Mechanical, Optical, Wireless |
| **Touchpad** | Pointing device on laptops; touch-sensitive pad moves cursor |
| **Graphic Tablet** | Input for drawing images/graphics; like pencil on paper |
| **Gamepad** | Controller for computer/console gaming systems |
| **Scanner** | Reads text/graphics from paper; types: Flatbed, Handheld |
| **Barcode Reader** | Reads product barcodes; used in supermarkets, showrooms |

- I/O devices are also called **peripheral devices** (surround CPU and memory)
- ATM example inputs: smart card, keyboard, touch screen
- OCR (Optical Character Recognition) reads printed/handwritten text
- MICR (Magnetic Ink Character Recognition) reads bank cheque codes
- Light pen: selects and displays objects on screen (used with graphics)

**Input Device Selection Guide**

| Need | Best Device |
|------|-------------|
| Typing text/data | Keyboard |
| Pointing/clicking on screen | Mouse or Touchpad |
| Drawing/sketching | Graphic Tablet |
| Scanning printed document | Scanner (Flatbed/Handheld) |
| Reading product codes | Barcode Reader |
| Gaming controls | Gamepad |
| Touch-based input (ATM, kiosk) | Touch Screen |

**For Exam**
Input devices accept data and instructions from the user. The keyboard is the most common standard input device with QWERTY layout. Mouse and touchpad are pointing devices for cursor control. Scanner converts printed text/graphics to digital form. Barcode reader reads product barcodes in retail. Other devices include graphic tablet, gamepad, light pen, and OCR/MICR devices.

**Diagram (refer SLM):** Fig. 1.3.1 Keyboard; Fig. 1.3.2 Mouse; Fig. 1.3.3 Touchpad; Fig. 1.3.4 Graphic Tablet; Fig. 1.3.5 Gamepad; Fig. 1.3.6 Scanner; Fig. 1.3.7 Barcode Reader.

#### 1.3.2 Output Devices ⭐

**Theory**
Output devices communicate processed information back to the user. They are broadly classified into soft copy devices (monitor, speakers — visible/audible only while device is on, editable) and hard copy devices (printers, plotters — permanent physical output). Output types include text, graphics, audio, video, and tactile. Printers are categorized as impact (touches paper: daisy wheel, dot matrix) and non-impact (no contact: laser, inkjet).

**Important Points**

| Device | Type | Description |
|--------|------|-------------|
| **Monitor** | Soft copy | Visual display; CRT replaced by LCD, LED, OLED, Plasma; TFT-LCD/LED flat panels |
| **Multimedia Speaker** | Soft copy (audio) | Sound output for movies, games, music |
| **Printer** | Hard copy | Text/graphics on paper; Impact: Daisy wheel (letter quality, noisy), Dot matrix (cheap, low quality); Non-impact: Laser (fast, high quality), Inkjet |
| **Plotter** | Hard copy | Large-format graphs, engineering drawings, maps; types: Drum, Flatbed |

- Soft copy: available only when device is on; can be edited and saved
- Hard copy: permanent physical objects; cannot be edited after printing
- Dot matrix: serial and line dot-matrix types; laser printer uses rotating mirror
- Output types: Text, Graphics, Audio, Video, Tactile

**For Exam**
Output devices deliver processed results to users. Monitors provide soft copy visual output (LCD/LED/OLED). Speakers provide audio soft copy. Printers produce hard copy — impact printers (daisy wheel, dot matrix) touch paper; non-impact printers (laser, inkjet) do not. Plotters produce large-format engineering drawings and graphs. Soft copy is temporary and editable; hard copy is permanent.

**Diagram (refer SLM):** Fig. 1.3.8 Monitor; Fig. 1.3.9 Laser Printer; Fig. 1.3.10 Plotter.

### Unit Recap (from SLM)
- Input devices give data to the computer; output devices return processed information
- Keyboard = most common input device (QWERTY layout)
- Mouse and touchpad = pointing devices (point, drag, drop)
- Scanner reads paper documents; barcode reader reads product barcodes
- Monitor = soft copy visual output; printer/plotter = hard copy output
- Speakers = audio soft copy output
- Printers: Impact (daisy wheel, dot matrix) vs Non-impact (laser, inkjet)
- Plotter = large-format graphs and engineering drawings

### Unit 4: Different Types of Computing Systems

#### 1.4.1 Evolution of Computers

**Theory**
In ancient times, people used fingers, pebbles, and simple calculators for computations. Key milestones include the Abacus (counting device), Napier's Bones (John Napier, multiplication aid), Pascaline (Blaise Pascal, 1642 — first mechanical adding machine), punched cards (Herman Hollerith, ~1880), and Charles Babbage's Difference Engine (1822) and Analytical Engine (1842 — father of computers). The digital era began with Claude Shannon's binary system; ABC (Atanasoff-Berry Computer, 1942) was the first electronic computer using vacuum tubes. Transistors (1947), FORTRAN (1957), IC (1959), mainframe with IC (1960), Intel 1KB memory chip (1970), and first microcomputer (1975, H. Edward Roberts) followed.

**Important Points**

- **Abacus** → **Napier's Bones** → **Pascaline** (1642) → **Punched cards** (1880–1970s)
- **Charles Babbage** = father of computers; Difference Engine + Analytical Engine
- **Claude Shannon** suggested binary system in digital era
- **ABC** (Atanasoff-Berry, 1942) = first electronic computer; vacuum tubes
- **1947:** Transistors; **1957:** FORTRAN; **1959:** IC; **1960:** Mainframe with IC
- **1970:** Intel 1KB memory chip; **1975:** First microcomputer (H. Edward Roberts)

**Computer Generations Summary**

| Generation | Period | Technology | Key Development |
|------------|--------|------------|-----------------|
| Pre-electronic | Ancient–1800s | Manual/mechanical | Abacus, Napier's Bones, Pascaline |
| 1st | 1940s–50s | Vacuum tubes | ABC computer, ENIAC era |
| 2nd | 1950s–60s | Transistors (1947) | Faster, smaller; FORTRAN (1957) |
| 3rd | 1960s–70s | Integrated Circuits (1959) | Mainframe with IC (1960); Intel 1KB chip (1970) |
| 4th | 1970s–present | Microprocessors | First microcomputer (1975); personal computing era |
| 5th (modern) | 1980s–present | VLSI, AI, IoT | Smartphones, wearables, cloud computing |

**For Exam**
Computer evolution progressed from Abacus and Napier's Bones to Pascaline (1642, first mechanical adder). Charles Babbage is the father of computers (Difference Engine, Analytical Engine). The digital era introduced binary system (Claude Shannon) and ABC computer (1942). Transistors (1947), ICs (1959), and microcomputers (1975) led to modern computing.

**Diagram (refer SLM):** Fig. 1.4.2 Abacus; Fig. 1.4.3 Napier's Bones; Fig. 1.4.4 Pascaline; Fig. 1.4.5 Punched Cards.

#### 1.4.2 Characteristics and Classification by Operating Principle 🔥

**Theory**
Computers possess key characteristics: Automatic (works without human intervention once started), Speed (completes in seconds what humans take years), Accuracy (consistent precision), Diligence (no fatigue, same accuracy for millions of calculations), Versatility (payroll, inventory, billing — many tasks), Power of Remembering (stores any amount of data), No IQ (follows instructions only), No Feeling (no emotions), and Storage (built-in + secondary). By operating principle, computers are classified as Analog (continuous physical quantities), Digital (digits/binary), or Hybrid (both — e.g., hospital ICU, heart beat measurement).

**Important Points**

- **Characteristics:** Automatic, Speed, Accuracy, Diligence, Versatility, Power of Remembering, No IQ, No Feeling, Storage
- Speed measured in ms → μs → **nanoseconds** today; supercomputers in **MIPS** (Millions of Instructions Per Second)
- **Analog:** Continuous information; waves/physical quantities; e.g., thermometer, speedometer, petrol pump indicator
- **Digital:** Calculations with digits (binary); high accuracy; used in banking, education, insurance
- **Hybrid:** Speed of analog + accuracy of digital; e.g., hospital ICU, pacemakers, insulin meters

**For Exam**
Computer characteristics include automatic operation, high speed, accuracy, diligence (no fatigue), versatility, large storage capacity, no IQ (needs instructions), and no feelings. By operating principle: Analog computers use continuous physical phenomena (thermometer, speedometer); Digital computers use binary digits with high precision; Hybrid computers combine both qualities (hospital patient monitoring).

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


## Block 2: Instructions, Memory and Storage

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

#### 2.3.3 Virtual Memory 🔥

**Theory**
Virtual memory is an OS feature that compensates for physical RAM shortages by moving data pages between RAM and disk storage, allowing programs to believe they have more memory than physically available. It separates user logical memory from physical memory — programs run smoothly even with relatively small RAM. Physical addresses are hardware addresses in main memory; logical addresses are generated by the processor. Virtual address space is the virtual storage assigned to a process (program in execution).

**Important Points**

- Extends physical memory using disk; provides memory protection
- **Physical address:** hardware address in main memory
- **Logical address:** generated by processor
- **Virtual address:** allocated to virtual memory location accessed as if in main memory
- **Virtual address space:** virtual storage assigned to a process
- **Real address:** address of storage location in main memory
- OS swaps required program parts between main and secondary memory

**Virtual Memory — How It Works (Step by Step)**
1. Program requests more memory than physically available in RAM
2. OS divides program into **pages** (fixed-size blocks)
3. Required pages loaded into RAM; rest kept on disk (secondary storage)
4. When CPU needs a page not in RAM, a **page fault** occurs
5. OS swaps out less-used pages from RAM to disk, loads needed page into RAM
6. User/program sees a continuous large address space — unaware of swapping

**Address Types Summary**

| Address Type | Generated By | Refers To | Example Use |
|--------------|-------------|-----------|-------------|
| **Logical Address** | Processor (CPU) | Virtual memory location | Program's view of memory |
| **Virtual Address** | OS/MMU | Address in virtual address space | Mapped to physical or disk |
| **Physical Address** | Hardware (actual RAM) | Real location in main memory | Actual RAM chip location |
| **Real Address** | — | Storage location in main memory | Same as physical address |

**For Exam**
Virtual memory allows running large programs on computers with limited RAM by using disk as extension of main memory. The OS manages swapping between primary and secondary storage. Physical addresses are actual hardware memory locations; logical addresses are processor-generated. Virtual address space is assigned per process. This separation of logical and physical memory enables efficient memory management and protection.

**Diagram (refer SLM):** Fig. 2.3.5 Applications (TV app store analogy for virtual memory).

### Unit Recap (from SLM)
- Registers: fastest storage; Data, Address, Status types
- MAR (address), MDR (data), Accumulator (ALU results), PC (next instruction), IR (current instruction)
- Condition Code Register with 1-bit flags
- Cache L1/L2/L3; hit ratio = hits/(hits+misses)
- Virtual memory extends RAM using disk; virtual vs physical/logical addresses

### Unit 4: Secondary Storage Devices

#### 2.4.1 Secondary Storage and Magnetic Storage

**Theory**
Secondary storage provides cheap, non-volatile, large-capacity permanent storage since primary memory is expensive, limited, and volatile. The processor needs primary memory for fast intermediate results during processing. Secondary storage characteristics: non-volatile, large size, cheaper than primary memory. Devices are fixed (hard disk drive) or removable (pen drive, optical discs). Magnetic storage stores data on magnetic medium using magnetization patterns — either sequential access (magnetic tape) or direct/random access (magnetic disk).

**Important Points**

| Type | Access | Description | Capacity/Speed |
|------|--------|-------------|----------------|
| **Magnetic Tape** | Sequential | Older; backup; high recording density; low cost per bit | Large data; portable; sequential only |
| **Hard Disk (HDD)** | Random | Main data storage; metal/plastic disks with iron oxide coating | 4500–7200 rpm; GB–TB; ms access time |
| **Floppy Disk** | Random | Oldest portable; obsolete | 1.44 MB standard |

- Secondary storage: non-volatile, large, cheap permanent storage
- Primary memory still needed for speed during processing
- HDD stores data using magnetization patterns on disk

**For Exam**
Secondary storage provides non-volatile, large, inexpensive permanent storage. Magnetic storage uses magnetization on magnetic medium. Magnetic tape is sequential access, used for backup. Hard disk (HDD) is the main random-access storage device with rpm 4500–7200 and capacity in GB–TB. Floppy disk (1.44 MB) is obsolete. Fixed devices include HDD; removable include pen drives and optical discs.

**Diagram (refer SLM):** Fig. 2.4.1 Secondary Storage Devices; Fig. 2.4.2 Magnetic Tape; Fig. 2.4.3 Hard Disk; Fig. 2.4.4 Floppy Disk.

#### 2.4.2 Optical Storage

**Theory**
Optical discs store data read and written by lasers, with much higher capacity than floppies. CD (Compact Disc, invented by James Russell, first produced 1982) holds 650–700 MB; types include CD-R (write once) and CD-RW (rewritable). DVD (Digital Versatile/Video Disc) holds 4.7–17 GB depending on layers/sides. Blu-ray uses blue laser with shorter wavelength for high-definition content — single layer 25 GB, dual layer 50 GB.

**Important Points**

| Media | Capacity | Key Features |
|-------|----------|--------------|
| **CD** | 650–700 MB (80-min) | CD-R (record once), CD-RW (rewritable); Nero software for burning |
| **DVD** | 4.7 GB (single-layer) to 17.08 GB (double-sided double-layer) | DVD-R (write once), DVD-RW (erasable) |
| **Blu-ray (BD)** | 25 GB (single layer), 50 GB (dual layer) | Blue laser; HD content; 3D movies |

**For Exam**
Optical storage uses lasers to read/write data. CD holds 650–700 MB (CD-R write once, CD-RW rewritable). DVD stores 4.7–17 GB for movies and data. Blu-ray uses blue laser for HD content — 25 GB single layer, 50 GB dual layer. Optical discs replaced floppies due to higher capacity.

**Secondary Storage — Complete Capacity Comparison Table**

| Device | Type | Capacity | Access | Media/Technology | Status / Notes |
|--------|------|----------|--------|------------------|----------------|
| **Floppy Disk** | Removable | 1.44 MB | Random | Magnetic disk | Obsolete; replaced by USB/optical |
| **CD (Compact Disc)** | Removable | 650–700 MB | Random | Optical (laser) | CD-R (write once), CD-RW (rewritable) |
| **DVD (single-sided, single-layer)** | Removable | 4.7 GB | Random | Optical (laser) | Movies, software distribution |
| **DVD (single-sided, dual-layer)** | Removable | 8.5–8.7 GB | Random | Optical (laser) | Extended movie storage |
| **DVD (double-sided, single-layer)** | Removable | 9.4 GB | Random | Optical (laser) | Both sides used |
| **DVD (double-sided, dual-layer)** | Removable | up to 17.08 GB | Random | Optical (laser) | Maximum DVD capacity |
| **Blu-ray (single layer)** | Removable | 25 GB (~2 hr HD video) | Random | Optical (blue laser) | HD/3D movies; shorter wavelength |
| **Blu-ray (dual layer)** | Removable | 50 GB (~4.5 hr HD video) | Random | Optical (blue laser) | Latest 3D movies on Blu-ray only |
| **HDD (Hard Disk Drive)** | Fixed/Removable | GB – TB (typ. 500 GB–16 TB) | Random | Magnetic disk | 4500–7200 rpm; ms access time |
| **SSD (Solid State Drive)** | Fixed/Removable | GB – TB (typ. 256 GB–4 TB) | Random | NAND flash memory | Faster, lower power, no moving parts |
| **Pen Drive (USB Flash)** | Removable | 8 GB – 512 GB+ | Random | USB flash (NAND) | Portable; scratch/magnetic resistant |
| **External HDD** | Removable | TB (typ. 1–8 TB) | Random | Magnetic disk | Best for backup; USB connected |
| **Memory Stick** | Removable | Varies (MB–GB) | Random | Flash (Sony) | Cameras; compact, no moving parts |
| **Magnetic Tape** | Removable | TB+ | Sequential | Magnetic tape | Backup/archival; low cost per bit |

**DVD Capacity Breakdown (from SLM)**

| DVD Structure | Capacity |
|---------------|----------|
| Single-sided, single-layer | 4.7 GB |
| Single-sided, double-layer | 8.5 – 8.7 GB |
| Double-sided, single-layer | 9.4 GB |
| Double-sided, double-layer | up to 17.08 GB |

**Blu-ray Capacity Breakdown (from SLM)**

| Blu-ray Type | Capacity | Content Equivalent |
|--------------|----------|-------------------|
| Single layer | 25 GB | ~2 hours HD video or ~13 hours standard video |
| Dual layer | 50 GB | ~4.5 hours HD video or ~20 hours standard video |

**SSD vs HDD Quick Comparison**

| Feature | HDD | SSD |
|---------|-----|-----|
| Technology | Magnetic disk (spinning platters) | NAND flash (no moving parts) |
| Speed | Slower (ms access) | Much faster (μs access) |
| Capacity | Higher (up to 16+ TB) | Lower per cost (typ. up to 4 TB) |
| Power | Higher consumption | Lower consumption |
| Reliability | Sensitive to shock | Shock resistant |
| Cost per GB | Lower | Higher (decreasing) |
| Best for | Bulk storage, backup | OS drive, laptops, performance |

#### 2.4.3 USB, Pen Drive, External HDD, Memory Stick, and SSD

**Theory**
USB (Universal Serial Bus) is an industry standard interface with Type A, B, and C ports connecting peripherals like cameras, smartphones, and printers. Pen drives are USB flash storage devices for documents, photos, music, and video. External HDDs are portable high-capacity (terabytes) backup devices connected via USB. Memory sticks (introduced by Sony for cameras) are compact removable flash media. SSDs (Solid State Drives) use NAND flash for faster, lower-power, more reliable storage than traditional HDDs.

**Important Points**

| Device | Description | Advantages |
|--------|-------------|------------|
| **USB** | Universal Serial Bus; industry standard port interface | Type A, B, C ports; connects peripherals |
| **Pen Drive** | USB flash storage; pen-shaped | Scratch/dust/magnetic resistant; low power; portable; affordable |
| **External HDD** | Outside computer with own enclosure; USB connected | High capacity (TB); backup; portable; easy to use |
| **Memory Stick** | Sony portable flash media for cameras | Compact; large capacity; no moving parts; durable |
| **SSD** | NAND flash secondary storage | Faster, less power, more reliable than HDD; portable or internal |

**For Exam**
USB is the standard interface for connecting devices. Pen drives are USB flash storage for files and media. External HDDs provide terabyte backup capacity via USB. Memory sticks are Sony's compact flash media. SSDs use NAND flash, offering faster access, lower power consumption, and greater reliability than HDDs, though at higher cost per gigabyte.

**Diagram (refer SLM):** Fig. 2.4.5 Pen Drive; Fig. 2.4.6 Memory Stick.

### Unit Recap (from SLM)
- Secondary storage: non-volatile, large, cheap permanent storage
- Magnetic: tape (sequential, backup), disk/HDD (random, main storage), floppy (1.44 MB, obsolete)
- Optical: CD (650–700 MB), DVD (4.7–17 GB), Blu-ray (25–50 GB, blue laser)
- USB = Universal Serial Bus; pen drive = USB flash storage
- External HDD = backup; Memory stick = Sony portable media
- SSD = NAND flash, faster and more reliable than HDD


## Block 3: Software

### Unit 1: System Boot up and Software Layers

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

#### 3.1.2 Files and Folders ⭐

**Theory**

Files and folders form the foundational framework for organising digital data on computers. A **file** is a digital container storing text, images, audio, video, or programs — identified by name and extension (e.g., `Notes.doc`, `Image.jpg`). A **folder** (directory) groups related files hierarchically; nested folders create subdirectories. The wardrobe analogy: items = files, wardrobe = folder, drawers = subfolders.

**Important Points**

- File = name + extension (extension identifies type); **Path** = folder hierarchy (e.g., `C:\Users\Name\Documents\file.txt`)
- Examples: `Notes.doc` (Word), `Image.jpg` (JPEG), `document.txt` (text file)
- **File system** = software managing storage organisation on HDD/SSD
- **File operations:** create, open, edit, move, copy, delete, rename
- **Permissions** control access, modify, delete rights per user/group
- **Metadata** = data about data (size, creation date, modification date, author)
- Folders/directories group related files; nested subfolders create hierarchy (music/melody/fast)

**For Exam**

Files are digital storage units with name and extension identifying type. Folders (directories) group related files in a hierarchical structure with paths showing location. The file system manages organisation on storage devices. Users perform create, open, edit, move, copy, delete, and rename operations. Permissions and metadata (data about data) support security and file management.

#### 3.1.3 Booting and POST 🔥

**Theory**

**Booting** is the startup sequence that loads the OS when the computer is turned on — like a gym warm-up before exercise. During booting, the system checks all installed hardware/software and loads necessary files for operation. **POST** (Power On Self Test) runs early in booting to verify RAM, hard drives, CD-ROM, keyboard, and other components. **BIOS** (Basic Input Output System) supports booting from HDD, optical drives, and USB.

**Important Points**

| Type | Also Called | Description |
|------|-------------|-------------|
| Warm booting | Soft reboot | Restart without cutting power; skips full hardware re-init |
| Cold booting | Hard booting | Start from completely off state; full POST and initialization |

**Boot Process Steps (in order):**

| Step | Stage | What Happens |
|------|-------|----------------|
| 1 | Power On | User presses power button; electricity supplied to components |
| 2 | BIOS/UEFI Init | Firmware starts; configures basic hardware settings |
| 3 | POST | Tests RAM, drives, keyboard, CD-ROM; beeps/error codes on failure |
| 4 | Boot Device Selection | BIOS scans boot order (HDD → optical → USB) for bootable media |
| 5 | Boot Loader Load | Small program loaded from boot device into memory |
| 6 | OS Kernel Load | Core OS files loaded into RAM — first layer of system software |
| 7 | Driver & Service Init | OS loads device drivers, starts essential background services |
| 8 | Ready State | Login screen or desktop appears; user can interact with system |

- Boot devices: hard disks, optical drives, USB (configured in BIOS boot order)
- POST failure halts boot — system displays error codes or audible beeps
- OS is the first major software loaded into memory at startup
- Warm boot reloads OS without full power cycle; cold boot runs complete POST

**For Exam**

Booting is the startup sequence loading the OS when the computer turns on. Steps: power on → BIOS init → POST (hardware test) → boot device selection → boot loader → OS kernel → drivers/services → ready state. POST verifies RAM, drives, keyboard, and components. BIOS supports booting from HDD, optical, and USB. Warm booting (soft reboot) restarts without cutting power; cold booting (hard booting) starts from off with full POST and initialization.

#### 3.1.5 Software Layers and Architecture 🔥

**Theory**

Software applications use three layers: **Presentation** (UI/client layer — user interaction), **Application** (business logic — processing between UI and data), and **Data** (storage layer). Gmail login page = presentation; login validation = application; user database = data. These layers deploy in **one-tier** (all on one machine), **two-tier** (client + data server), or **three-tier** (client + application server + data server) architectures.

**Important Points**

| Architecture | Layers Location | Example |
|--------------|-----------------|---------|
| One tier | All three in single package | MP3 player, standalone MS Office |
| Two tier | Client: presentation + application; Server: data | Client-server apps |
| Three tier | Client: presentation; App server: logic; DB server: data | Scalable web apps |

- Presentation layer (client layer): topmost; user interacts — Gmail login boxes/buttons
- Application layer (business logic): intermediate; processes login, queries database
- Data layer: stores and retrieves data for application layer
- One-tier: MP3 player, standalone MS Office — all layers in one package on one machine
- Two-tier: client handles presentation + application; server handles database; client requests, server responds
- Three-tier: client (UI) + application server (logic) + database server (data) — best scalability

**For Exam**

Three-tier architecture separates Presentation (client UI), Application (business logic on app server), and Data (database server) onto three distinct systems. Client handles only the user interface; application server processes requests and queries the database; database server stores and retrieves data. This provides better scalability than one-tier (all local) or two-tier (client + DB server) because each tier can be upgraded independently. Gmail, banking apps, and e-commerce sites commonly use three-tier design.

### Unit Recap (from SLM)
- Software classified into **System Software** and **Application Software**
- **File** = storage unit with name + extension; **Folder/Directory** = organises files
- **Booting** starts OS; types: **Warm** (soft reboot) and **Cold** (hard booting)
- Boot steps: Power on → BIOS → POST → boot device → boot loader → OS kernel → ready
- **POST** = Power On Self Test; **BIOS** selects boot device (HDD, optical, USB)
- Architecture: **One tier**, **Two tier**, **Three tier**
- Layers: **Presentation**, **Application (Business Logic)**, **Data**
- **Metadata** = data about data; **Path** = file location in folder hierarchy

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

#### 3.2.1.4 Windows vs Linux and Mobile OS 🔥

**Theory**

Windows and Linux are commonly used GUI operating systems with different management styles. **Android** (Google, 2008) is built on Linux kernel for touch devices — partially open source, most-used OS overall. **iOS** (Apple) runs on iPhone, iPod, and iPad.

**Important Points**

| Feature | Linux | Windows |
|---------|-------|---------|
| Source | Open source | Licensed/proprietary |
| Cost | Free | Costly |
| Filename | Case-sensitive | Case-insensitive |
| Efficiency | More efficient | Less efficient |
| Security | More secure | Less secure |

- Android (Google, 2008): built on **Linux kernel**; touch-screen tablets/smartphones; partially open source; most-used OS overall
- iOS (Apple Inc.): iPhone, iPod, iPad; proprietary Apple ecosystem
- Other mobile OS: BlackBerry, Web, watchOS
- Windows: licensed, proprietary, case-insensitive filenames, less efficient, less secure
- Linux: open source, free, case-sensitive, more efficient, more secure

**For Exam**

Linux is open-source, free, case-sensitive, efficient, and more secure. Windows is licensed, costly, case-insensitive, and proprietary. Android (Google, Linux kernel) dominates mobile devices since 2008. iOS (Apple) powers iPhone, iPod, and iPad. Both Windows and Linux act as system managers coordinating application "workers."

#### 3.2.2 Graphical User Interface (GUI) ⭐

**Theory**

A user interface is required to interact with computers. **GUI** (Graphical User Interface) allows interaction through graphical icons and visual representations instead of typed commands. It offers a visual representation of OS commands and functions, making computers accessible to beginners.

**Important Points**

- GUI advantages over DOS: easier for beginners, visual icon representation of commands
- Drag-and-drop, cut-and-paste simplify information exchange between applications
- Users can explore options by pointing mouse at icons instead of memorising commands
- GUI offers visual feedback; reduces learning curve for non-technical users
- Windows and Linux both provide GUI; DOS remains command-line only

**For Exam**

GUI (Graphical User Interface) allows users to interact with electronic devices through graphical icons and visual representations instead of typed commands. It offers a visual representation of OS commands, making computers accessible to beginners. Advantages over DOS include drag-and-drop, cut-and-paste, and easy exploration of options using a mouse. Windows and Linux are widely used GUI operating systems; DOS requires memorising and typing commands.

### Unit Recap (from SLM)
- OS manages hardware; acts as interface between user and hardware
- **DOS** = disk-based, single-user, single-task, command-based
- **GUI** = graphical icons; easier than command interface
- Client-server: client requests, server responds (restaurant analogy)
- OS types with examples: Batch, Multitasking (UNIX), Multiprocessing (Win NT), Real-Time (space), Distributed (cloud), Network (Win Server), Mobile (Android/iOS)
- **Windows** = licensed/proprietary; **Linux** = open source/free
- **Android** = Google, Linux kernel, 2008; **iOS** = Apple, iPhone/iPad

### Unit 3: System Software and Utilities

#### 3.3.1 Programming Languages 🔥

**Theory**

Programming languages are formal languages programmers use to communicate with computers. **High-level languages** (C, C++, Java, Python) use human-readable syntax and are portable. **Low-level languages** are machine-friendly: **Assembly** uses mnemonics (short codes); **Machine language** uses binary (0 and 1) — the only language computers directly understand.

**Important Points**

| Feature | High Level | Low Level |
|---------|------------|-----------|
| Nature | Programmer-friendly | Machine-friendly |
| Memory | Less efficient | Highly efficient |
| Understanding | Easy | Tough |
| Debugging | Simple | Complex |
| Portability | Portable | Non-portable |

- Assembly language uses **mnemonics** (short codes); more user-friendly than machine language
- Machine language = binary using only **0 and 1**; only language computer understands directly
- Writing binary programs is tedious — programmers prefer high-level languages + translators
- System software includes language translators, OS, and utilities making computer functional
- Department analogy: computer = department, HOD = system software, teachers = applications

**For Exam**

Programming languages are formal languages for programmer-computer communication. High-level languages (C, C++, Java, Python) are programmer-friendly, portable, and easier to debug. Low-level languages are machine-friendly and memory-efficient: assembly uses mnemonics (short codes); machine language uses binary (0 and 1) — the only language computers understand. Translators bridge the gap: compiler (whole program), interpreter (line by line), assembler (assembly to machine). Programmers prefer high-level languages because writing binary is tedious.

#### 3.3.2 Language Translators 🔥

**Theory**

Computers understand only machine language; programmers write in high-level languages. **Language translators** convert programs to machine-understandable form. **Compiler** converts entire program at once; **Interpreter** translates line by line; **Assembler** converts assembly language to machine language.

**Important Points**

| Feature | Compiler | Interpreter |
|---------|----------|-------------|
| Translation | Entire program at once | Line by line |
| Analysis time | More | Less |
| Execution time | Less | More |
| Debugging | Harder | Easier |
| Object code | Generated | Not generated |
| Examples | C, C++, Java | Python, Perl, PHP |

- **Assembler** = assembly language → machine language; uses mnemonics (short codes)
- Compiler: analyses entire source before execution; generates intermediate object code
- Interpreter: analyses less but executes slower overall; no object code file
- C, C++ use compilers; PHP, Python use interpreters
- Hierarchy: High level → (Compiler/Interpreter) → Machine language; Assembly → (Assembler) → Machine language

**For Exam**

Language translators bridge high-level programs and machine language. A compiler translates the whole program before execution (C, C++ — faster execution, harder debugging). An interpreter translates line by line (Python, PHP — easier debugging, slower execution). An assembler converts assembly language to machine code.

#### 3.3.3 Database and DBMS

**Theory**

A **database** is a collection of information organised so programs can quickly select desired data — like a spice rack in a kitchen or telephone directory online. **DBMS** (Database Management System) is a set of programs enabling users to access, manipulate, report on, and represent data.

**Important Points**

- DBMS stores/retrieves data in multiple ways; balances needs of multiple applications
- Consistent data administration processes across organisation
- Sophisticated functions for efficient storage and retrieval
- Provides **Data Integrity** (accuracy) and **Security** (access control)
- Examples: online telephone directory, Facebook member/event/message data
- Kitchen spice rack analogy: organised data easy to select when needed

**For Exam**

A database is an organised electronic collection of data enabling quick selection — like a kitchen spice rack or online telephone directory. Facebook stores member, event, message, and advertising data in databases. DBMS (Database Management System) manages access, manipulation, reporting, and security. Advantages: stores large volumes, easy access/update, accurate data, consistent administration, balances multiple applications sharing data, and provides data integrity and security through sophisticated storage/retrieval functions.

#### 3.3.4 Utility Software

**Theory**

Utility software assists the OS in specialised maintenance tasks — analysing, configuring, and maintaining computers. It runs in support of system software and helps keep the system functional and secure.

**Important Points**

- Utility software = application software assisting OS in specialised tasks
- **Antivirus:** scans for boot viruses, Trojans, worms, spyware; removes/isolates threats
- **Backup software:** creates copies stored in secure location for data recovery
- **Debuggers:** test and debug other programs; fix programming errors
- **Disk checkers:** scan operating hard drives for errors
- **Disk cleaners:** find unnecessary files when hard disk is full; user decides what to delete
- **Disk compression:** transparently compress/decompress disk contents; increases capacity
- **Disk defragmenters:** detect scattered file fragments; rearrange for efficiency

**For Exam**

Utility software assists the OS in system maintenance and specialised tasks. Examples include antivirus (virus-free environment), backup (data copies), debuggers (fix program errors), disk checkers, disk cleaners, disk compression, and disk defragmenters. Antivirus is a key utility protecting against boot viruses, Trojans, worms, and spyware.

### Unit Recap (from SLM)
- System software controls and manages hardware; provides platform for applications
- **High level** (C, Java, Python) = programmer-friendly, portable; **Low level** (Assembly, Machine) = machine-friendly
- **Assembly** uses mnemonics; **Machine language** uses only 0 and 1
- **Compiler:** whole program → machine language (C, C++); **Interpreter:** line-by-line (Python, PHP)
- **Assembler:** assembly → machine language
- **Database:** organised information; **DBMS** manages access, integrity, security
- **Utility software:** antivirus, backup, debuggers, disk checkers/cleaners/compression/defragmenters
- System software analogy: HOD manages department; teachers = applications

### Unit 4: Application Software

#### 3.4.1 Application Software Types ⭐

**Theory**

Application software (end-user program) helps users perform specific tasks — takes user input and completes work. Types include word processing, spreadsheet, presentation, multimedia, database, and simulation software. **LaTeX** is a free document preparation system for high-quality scientific/technical documentation, separating content from style.

**Important Points**

| Type | Purpose | Examples |
|------|---------|----------|
| Word processor | Create, manipulate, store text | MS Word, Google Docs |
| Spreadsheet | Calculations in rows/columns/cells | MS Excel, Google Sheets |
| Presentation | Display info on slides | MS PowerPoint, Impress |
| Multimedia | Audio/video handling | Media players |
| Database | Data management apps | MS Access |
| Simulation | Model real-world scenarios | Flight simulators |

- Word processor features: create/save/edit, font/alignment/colour formatting, spell-check, images, headers/footers, watermarks
- Spreadsheet: rows × columns = cells; data as text/date/time/number; arithmetic, logical, text ops; charts/graphs
- Spreadsheet activities: addition, average, counting, charts, data entry, cell formatting, logical comparisons
- Presentation: info broken into slides; add text, graphics, video, images; conveys concept to audience
- LaTeX features: journal articles, technical reports, books, slide presentations; complex math formulas (AMS-LaTeX)
- LaTeX: cross-references, tables, figures, bibliographies, indexes, multilingual typesetting, artwork; separates content from style
- Specific purpose examples: GIMP, Payroll System, Airline Reservation, Tally, Inventory/HRM systems

**For Exam**

Application software (end-user program) performs specific tasks for users. Word processors (MS Word, Google Docs) create, format, and store text with spell-check and images. Spreadsheets (Excel) use rows, columns, and cells for calculations, charts, and logical comparisons. Presentation tools (PowerPoint) display information on slides with graphics and video. LaTeX is free scientific documentation software separating content from style, supporting math formulas and bibliographies. Other types: multimedia, database, simulation, and customised software (payroll, Tally).

#### 3.4.2 Computer Virus and Protection 🔥

**Theory**

A **computer virus** is malicious code that changes how a computer works and spreads between machines, damaging devices or stealing data. Entry methods include file sharing, infected webpages, and spam email attachments. Types: worms, Trojan, ransomware. Protection uses antivirus (utility software), firewall, and safe practices.

**Important Points**

- Virus types: **Worms** (self-replicating), **Trojan** (disguised malware), **Ransomware** (locks data for payment)
- Problems after infection: slow performance, frequent crashes, data loss/corruption, identity theft
- **Antivirus** = utility software scanning and eliminating viruses
- **Firewall** = network security device filtering traffic per organisation security policy
- Protection measures: use antivirus + firewall, update both frequently, update OS regularly
- Increase browser security settings; download only from trusted sites; avoid spam attachments

**For Exam**

A computer virus is malicious spreading code altering computer operation. Entry via file sharing, infected sites, or spam attachments causes slowdowns, crashes, data loss, and identity theft. Types include worms, Trojan, and ransomware. Protection requires antivirus utility software, firewall (network traffic filter), frequent updates, and downloading from trusted sources only.

### Unit Recap (from SLM)
- Application software = end-user program for specific tasks (MS Office, Tally)
- Types: Word Processing, Spreadsheet, Presentation, Multimedia, Database, Simulation
- Word processor: create/edit/format text; Spreadsheet: rows × columns × cells for calculations
- Presentation: slides with text, graphics, video; LaTeX: free scientific/technical documentation
- LaTeX separates content from style; supports math formulas, bibliographies, multilingual typesetting
- **Computer virus** = malicious spreading code; entry via files, infected sites, spam
- Virus types: Worms, Trojan, Ransomware; protection: antivirus, firewall, updates, trusted downloads


## Block 4: Networks and Internet

### Unit 1: Basic Concepts and Devices

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

### Unit 2: World Wide Web and Search Engines

#### 4.2.1 History of the Internet

**Theory**

The Internet evolved from US defense research. **ARPA** (1958) led to **ARPANET** (1962, J.C.R. Licklider). Packet switching (1965), TCP adoption (1983), **NSFNET** (1985) connected universities. **Tim Berners-Lee** created **HTTP** (1989) — father of WWW. **Mosaic** browser (1993, NCSA). NSFNET decommissioned 1995; commercial ISP model emerged.

**Important Points**

- 1958: ARPA created for US defense; physical cable networks
- 1962: J.C.R. Licklider proposed ARPANET for nuclear-attack-resistant communication
- 1965: Packet switching introduced; Stanford used first LAN for distant workstations
- 1981: ARPANET extended to national computer science researchers
- 1983: ARPANET adopted TCP; spread to university campuses; acted as early ISPs
- 1985: NSFNET connected university CS departments; linked supercomputing centers
- 1989: Tim Berners-Lee (CERN) created HTTP — father of WWW
- 1990: ARPANET gradually phased out
- 1993: Mosaic browser (NCSA) — key development from NSFNET era
- 1995: NSFNET decommissioned; commercial ISP model and Internet commerce emerged

**For Exam**

Internet history: ARPA (1958) → ARPANET (1962) → packet switching (1965) → TCP (1983) → NSFNET (1985) → HTTP/WWW by Tim Berners-Lee (1989) → Mosaic browser (1993) → commercial ISPs (post-1995). Tim Berners-Lee is the father of WWW; Mosaic was the key 1993 browser development.

#### 4.2.2 Internet and World Wide Web 🔥

**Theory**

The **Internet** is a global network of millions of computers sharing resources via ISPs, hardware, and wireless/cabling technologies. The **WWW** is a vast collection of linked information on web pages — the most common Internet information system. A **web page** is a single document; a **website** is a collection of pages with a common domain name on a web server.

**Important Points**

- Internet working (email example): Laptop A → ISP1 → Email Server A → Internet → ISP2 → Server B → Laptop B
- ISPs (MTNL, BSNL, Airtel, Jio) = companies offering Internet access for global data transfer
- WWW = vast linked information on web pages; most common Internet information system
- Encyclopaedia analogy: WWW = whole book; web page = one page you turn to
- Web page built with HTML (structure), CSS (design), JavaScript (interactivity)
- **Website working (4 steps):** browser requests page → Internet forwards to web server → server sends HTML → browser displays page
- **Static website:** fixed content, same for every user, infrequent design changes
- **Dynamic website:** content changes each visit; may differ per user (e.g., Facebook feed)
- **Web server** stores, processes, delivers pages; **Intranet server** = internal, not public

**For Exam**

Internet is a global network of millions of computers connected via ISPs for resource sharing and communication. ISPs (BSNL, Airtel, Jio) are the essential link between your device and remote servers. WWW is a vast linked collection of web pages — like an encyclopaedia where each page holds text, images, and hyperlinks. A web page is built with HTML (structure), CSS (design), JavaScript (interactivity); a website is a collection with a common domain on a web server. Static sites show fixed content; dynamic sites change per visit or user (e.g., social feeds). Website access: browser requests → Internet → web server → HTML returned → displayed.

#### 4.2.3 Websites — Static vs Dynamic ⭐

**Theory**

A **website** is a collection of web pages with a common domain name published on a web server by an individual, business, or institution. Pages are accessed via Internet using URLs. Websites classify as **static** (fixed content, same for every user) or **dynamic** (content changes each visit, may differ per user).

**Important Points**

- **Static:** web pages loaded exactly as stored; infrequent content/design changes; built with HTML
- **Dynamic:** portions change without full page reload; HTML + JavaScript; per-user content (e.g., news feed)
- **Web server** stores, processes, delivers pages; internal-only server = **Intranet server**
- Website access flow: browser request → Internet → web server → HTML page → browser display
- Example static: institutional brochure site; example dynamic: Amazon, Facebook

**For Exam**

A website is a collection of web pages sharing a domain name, published on a web server. Static websites display fixed content identical for every user, created mainly with HTML. Dynamic websites change content on each visit or per user using HTML and JavaScript. Access flow: browser sends request via Internet, web server returns HTML, browser renders the page. Intranet servers serve internal organisational pages not visible to the public.

#### 4.2.5 URL and Browsers 🔥

**Theory**

**URL** (Uniform Resource Locator) is a unique web address pointing to one specific page or file — like a postal address. Parts: protocol (https), WWW, domain name (www.google.com), extension (.com), and page name. A **browser** is software to access and view websites (Chrome, Firefox, Safari, IE).

**Important Points**

- URL example: `https://www.google.com/doodle`
- **https** = protocol rules for browser-computer communication over Internet
- **www** = World Wide Web prefix
- **www.google.com** = domain name (registered to one owner; points to root directory)
- **.com** = extension indicating owner type (.gov, .co.uk also common)
- **doodle** = specific page/file on the website
- Browser features: back/forward navigation, refresh (reload), stop (cancel loading), home (preset page)
- Address bar: enter URLs; dropdown of previously visited sites; tabbed browsing for multiple sites
- Bookmarks save URL addresses; web search tool lets you choose favourite search engine

**For Exam**

URL is a unique web address directing the browser to a specific page — like a postal address for mail. Example `https://www.google.com/doodle`: **https** = communication protocol; **www** = World Wide Web; **google.com** = registered domain name; **.com** = extension (owner type); **doodle** = specific page. Browsers (Chrome, Firefox, Safari, IE) access websites with navigation buttons, address bar, refresh/stop, home, tabs, bookmarks, and built-in search. Bookmarks save URLs; tabbed browsing opens multiple sites in one window.

#### 4.2.7 Search Engines and Search Tips 🔥

**Theory**

A **search engine** is Internet software querying an indexed database and returning best-matching results. It uses a **web crawler/spider** to systematically index downloaded pages (like a librarian cataloguing books). Tips: specific keywords, quotation marks for exact phrases, Boolean +/- operators, Google Advanced Search, browser history, and Ctrl+F on pages.

**Important Points**

- Search engine analogy: library = search engine, librarian = browser, user = searcher
- Crawler/spider systematically indexes downloaded pages using algorithms for fast retrieval
- Search does NOT go directly to web — queries pre-built index database first
- Results show page title, text portion size, images, videos
- **Keywords:** be specific (search "lotus" not generic "flower")
- **Quotation marks:** `"Maruti Car Service"` for exact phrase match
- **Boolean:** `+` include, `-` exclude — `"Maruti Car Service"+Kerala-jobs`
- **Advanced Search:** filter by date, country, language, amount
- **Browser History:** revisit previously viewed pages
- **Ctrl+F:** find word/phrase within an already-open web page

**For Exam**

Search engines (Google, Yahoo, Bing) are Internet software querying a pre-built indexed database — they do not search the live web directly. A web crawler/spider systematically downloads and indexes pages (like a librarian cataloguing books). Tips: use specific keywords, quotation marks for exact phrases (`"Maruti Car Service"`), Boolean operators (`+Kerala -jobs`), Google Advanced Search for date/country filters, browser history for revisiting pages, and Ctrl+F to find text on an open page. Results include page title, text size, images, and videos.

### Unit Recap (from SLM)
- Internet launched 1958 (ARPA); **ARPANET** (1962), **TCP** (1983), **NSFNET** (1985), **HTTP** (1989)
- **Tim Berners-Lee** = father of WWW; **Mosaic** = 1993 browser; NSFNET decommissioned 1995
- **Internet** = global network via ISPs; **WWW** = linked web pages (encyclopaedia analogy)
- **Web page** = single document (HTML/CSS/JS); **Website** = collection on web server
- **Static** = fixed content; **Dynamic** = changes per visit/user
- **URL** = unique address (protocol + domain + extension + page)
- **Browser** accesses sites; **Search engine** + **crawler** query indexed database
- Search tips: keywords, quotes, Boolean (+/-), Advanced Search, Ctrl+F

### Unit 3: Internet Connectivity

#### 4.3.1 Internet Service Providers (ISP)

**Theory**

An **ISP** is a company offering Internet access — the gateway between your computer and all Internet servers. Without an ISP subscription, a computer with a modem cannot access the Internet. ISPs enable email, shopping, research, and all online activities.

**Important Points**

- ISP = gateway/link between your computer and all Internet servers
- Without ISP subscription, built-in modem alone cannot access Internet
- **Internet Access:** connecting PDA devices (phones, tablets) online; speed per plan
- **Domain Name Registration:** reserve unique name ~1 year (.com, .gov, .co.in); cannot buy lifetime
- **Web Hosting:** ISP rents space on web server for website files (pictures, audio, video)
- **Usenet:** collection of online discussion newsgroups; Q&A and file sharing forums
- Indian ISPs: BSNL, Airtel, Reliance Jio, Vodafone-Idea, MTNL
- Email route: your PC → ISP servers → destination ISP → recipient (ISP is essential link)

**For Exam**

ISP is the gateway to the Internet, offering access, domain registration, web hosting, and Usenet discussions. Internet access connects devices online at plan-dependent speeds. Domain registration reserves a unique name annually. Web hosting allocates server space for website files. Examples: BSNL, Airtel, Jio.

#### 4.3.2.1 Dial-up and Cable — Detail

**Theory**

**Dial-up** uses PSTN (Public Switched Telephone Network) landline with a modem to connect to an ISP. PSTN uses **circuit switching** — a dedicated physical path between sender and receiver. The modem converts digital computer data to analog for transmission and back to digital at the receiver. Common in remote areas where broadband is unavailable.

**Important Points**

- Setup: PC A → modem → telephone line → ISP → Internet cloud → ISP → modem → PC B
- Modem = Modulator-Demodulator; converts digital ↔ analog signals
- Circuit switching: connection-oriented; dedicated path for entire session
- Phone line busy during dial-up session — cannot use phone and Internet simultaneously (unlike DSL)
- Cable modem: ISP is cable TV operator; coaxial or fibre to home outlet

**For Exam**

Dial-up connection uses PSTN landline and modem with circuit switching to reach an ISP. The modem converts digital data to analog for telephone transmission and reconverts at the receiver. It suits remote areas lacking broadband but offers very slow speeds (up to 56 Kbps). Cable modem uses coaxial/fibre from a cable TV operator with a splitter providing separate TV and Internet connections.

#### 4.3.2.3 Wireless Local Loop (WLL)

**Theory**

**WLL** connects the subscriber to the nearest telephone exchange via a **radio link** instead of copper telephone lines — making it wireless unlike dial-up. Used where wired infrastructure is difficult. Main components: PSTN, Switch Function, WANU, and WASU.

**Important Points**

| Component | Role |
|-----------|------|
| PSTN | Circuit-switched global telephone network |
| Switch Function | At local exchange; routes PSTN among WANU units |
| WANU | Wireless Access Network Unit — authentication, routing, transceiving voice/data |
| WASU | Wireless Access Subscriber Unit — at subscriber home; connects to WANU via antenna |

- All local WASU units connect to WANU wirelessly through antenna
- WANU functions: Authentication, Operation & Maintenance, Routing, Transceiving
- WLL speed typically 128 Kbps–2 Mbps; moderate cost; wireless alternative to dial-up

**For Exam**

WLL (Wireless Local Loop) connects subscribers to the exchange using a radio link instead of telephone copper cables. Components: PSTN (circuit-switched network), Switch Function (at exchange), WANU (network-side unit handling authentication and routing), and WASU (subscriber-side unit with antenna). It provides wireless Internet access where wired lines are unavailable, with speeds typically below broadband but above dial-up.

#### 4.3.2.4 Digital Subscriber Line (DSL)

**Theory**

**DSL** uses existing telephone lines to transfer data and connect to the Internet. Operates on **different frequencies** for telephone voice and data — so phone and Internet work simultaneously without interruption. Two forms: **symmetric** (equal upload/download) and **asymmetric** (faster download, slower upload — most common for home users).

**Important Points**

- Setup: ISP → phone wall socket → DSL splitter → modem (Internet) + telephone (voice)
- Splitter separates frequencies: one band for voice calls, another for Internet data
- Symmetric DSL: equal speeds both directions (business use)
- Asymmetric DSL (ADSL): faster download — suited for browsing, streaming, downloads
- Dedicated continuous connection while line is active; speeds typically 1–100 Mbps

**For Exam**

DSL is an Internet connection using telephone lines at frequencies separate from voice calls, enabling simultaneous phone and Internet use via a DSL splitter. Symmetric DSL offers equal upload/download speeds; asymmetric DSL (ADSL) offers faster downloads for typical home use. ISP provides connection to the phone socket; splitter routes voice to telephone and data to DSL modem and computer.

#### 4.3.2.5 Fibre Optics — Detail

**Theory**

**Fibre optics** converts electrical signals carrying information into light pulses transmitted through transparent glass fibres about the diameter of a human hair. Speeds exceed DSL and cable — typically tens to hundreds of Mbps or Gbps. Core broadband technology for modern high-speed Internet (FTTH — Fibre To The Home).

**Important Points**

| Layer | Function |
|-------|----------|
| Outer jacket | Protects fibre from mechanical/environmental stress |
| Strength member | Additional mechanical protection |
| Coating | Extra protection for core and cladding |
| Cladding | Reduces light scattering; keeps light inside core |
| Glass core | Innermost; transmits light signals; larger core = more light capacity |

- Electrical signals → light → glass fibre → electrical at receiver
- Faster than DSL and cable modem; preferred for high-bandwidth needs
- Used by cable TV operators and ISPs for premium broadband plans

**For Exam**

Fibre optic technology converts electrical signals to light transmitted through glass fibres. Structure: outer jacket and strength member (protection), coating, cladding (prevents light escape), and glass core (transmits light). It delivers speeds far exceeding DSL and cable, making it the preferred broadband medium for high-speed Internet. Larger core diameter allows more light and higher data capacity.

#### 4.3.2 Internet Connection Types ⭐

**Theory**

ISPs provide connectivity through various technologies — from dial-up over telephone lines to high-speed broadband and dedicated leased lines. **Wired** connections use physical cables (copper, coaxial, optical fibre); **wireless** uses radio waves (Wi-Fi, WiMAX, satellite). Speed and cost vary by technology, coverage area, and whether bandwidth is shared or dedicated.

**Important Points**

| Connection | Technology | Typical Speed | Cost | Best For |
|------------|------------|---------------|------|----------|
| Dial-up | PSTN landline + modem; circuit switching | Up to 56 Kbps | Very low | Remote areas without broadband |
| Cable modem | Coaxial/fibre via cable TV operator | 10–500+ Mbps | Moderate | Homes with cable TV infrastructure |
| WLL | Radio link (WANU/WASU) to exchange | 128 Kbps–2 Mbps | Low–moderate | Areas lacking wired telephone lines |
| DSL | Telephone line; symmetric/asymmetric frequencies | 1–100 Mbps | Moderate | Homes/offices with existing phone lines |
| Fibre (FTTH) | Light signals through glass fibre core | 100 Mbps–1 Gbps+ | Moderate–high | High-speed urban/suburban areas |
| Wi-Fi | Short-range wireless via router + modem | Depends on ISP plan | Low (uses existing broadband) | Home/office local wireless access |
| WiMAX | Microwave radio; longer range than Wi-Fi | Up to 1 Gbps | Moderate | Sparsely populated / wide coverage |
| Satellite | Geostationary satellite + dish + modem | 12–100 Mbps (high latency) | High | Remote/rural with no terrestrial lines |
| BPL | Broadband over electrical power lines | Variable; emerging | Low potential | Limited pilot areas |
| Leased line | Dedicated symmetric bandwidth | 2 Mbps–10 Gbps | Highest | Businesses needing guaranteed SLA |

| Connection | Technology | Key Detail |
|------------|------------|------------|
| Dial-up | PSTN + modem | Analog conversion; circuit switching; phone line busy during use |
| Cable modem | Coaxial/fibre | Splitter: one to modem (Internet), one to set-top box (TV) |
| WLL | Radio link | WANU (network unit) + WASU (subscriber unit); wireless to exchange |
| Broadband | ≥25 Mbps down, 3 Mbps up (FCC) | Umbrella: fibre, wireless, cable, DSL, satellite, BPL |
| DSL | Phone line dual-frequency | Symmetric (equal up/down) or asymmetric (faster download) |
| Leased line | Dedicated pipe | Fixed bandwidth; no peak-time slowdown |

**Broadband sub-types:**

- **Fibre optics:** electrical → light through glass fibres; core transmits, cladding reduces scattering
- **Wi-Fi:** short-range wireless; router connects modem output to Wi-Fi devices
- **WiMAX:** Worldwide Interoperability for Microwave Access; longer range/speed than Wi-Fi

| Feature | Wi-Fi | WiMAX |
|---------|-------|-------|
| Range | Short (home/office) | Longer (city/rural coverage) |
| Speed | Depends on ISP plan | Up to 1 Gbps |
| Use | Local wireless access | Wide-area wireless broadband |
| Devices | Router + modem at home | Base station coverage area |

- **Satellite:** geostationary satellites; high latency but reaches anywhere with dish view
- **BPL:** broadband over power lines; avoids new cabling; very limited deployment
- WLL components: **PSTN** (circuit-switched telephone network), **Switch Function** (at local exchange), **WANU** (Wireless Access Network Unit — authentication, routing, transceiving), **WASU** (Wireless Access Subscriber Unit — at subscriber home)
- WLL: radio link replaces copper telephone lines; subscriber connects to exchange wirelessly via antenna
- Dial-up: digital→modem→analog→PSTN→ISP→Internet→reverse at receiver; modem converts both ways
- Satellite working: PC A → router → modem → dish → geostationary satellite → provider hub → web server → reverse path
- Satellite uses geostationary satellites (not telephone lines); dish + modem at subscriber; high latency
- BPL (Broadband over Powerline): Internet via existing electrical network; avoids new cabling; limited areas
- Compare cost: Dial-up (cheapest) < WLL < DSL/Cable < Fibre < Satellite < Leased line (most expensive)
- Compare speed: Dial-up (56 Kbps) < WLL < DSL < Cable < Fibre/WiMAX < Leased line (dedicated Gbps possible)

**For Exam**

Connection types vary in speed, cost, and suitability. Dial-up (56 Kbps, PSTN/modem, very cheap) suits remote areas. Cable modem (high Mbps via coaxial/fibre splitter) and DSL (phone line, symmetric/asymmetric) are common home options. Fibre offers fastest speeds via light in glass fibres. Wi-Fi provides local wireless; WiMAX covers wider areas. Satellite serves remote locations with higher latency and cost. WLL uses radio (WANU/WASU). Leased line gives dedicated symmetric bandwidth at highest cost for businesses. Broadband (≥25/3 Mbps per FCC) encompasses fibre, wireless, cable, DSL, satellite, and BPL.

#### 4.3.3 Leased Line

**Theory**

A **leased line** is a dedicated, fixed-bandwidth, symmetric data connection providing reliable high-quality Internet with assured upload and download speeds. Unlike shared connections, bandwidth does not fall at peak times.

**Important Points**

- Links office locations or computers/servers across sites (e.g., two branch offices)
- Reserved bandwidth for exclusive use — not shared with other ISP customers
- Carries Internet traffic, phone calls, and other data (dedicated pipe analogy)
- Bandwidth does NOT fall at peak times unlike ordinary shared connections
- Symmetric: equal upload and download speeds guaranteed
- Used where reliability and consistent speed are critical (banks, corporates, universities)

**For Exam**

A leased line is a dedicated, fixed-bandwidth, symmetric connection linking office locations with assured upload/download speeds. It provides reliable high-quality Internet without peak-time bandwidth reduction, unlike shared ISP connections. Used for inter-office linking with reserved bandwidth.

### Unit Recap (from SLM)
- **ISP** = gateway to Internet; services: access, domain registration, hosting, Usenet
- **Dial-up:** PSTN, circuit switching, modem; up to 56 Kbps; very low cost
- **Cable modem:** splitter for TV + Internet; moderate speed/cost
- **WLL:** radio link; WANU/WASU components; wireless to exchange
- **Broadband:** fibre, wireless (Wi-Fi/WiMAX), satellite, BPL, DSL; ≥25/3 Mbps
- **Fibre** = fastest; **Satellite** = remote areas; **Leased line** = dedicated symmetric bandwidth
- **Wi-Fi** = short range; **WiMAX** = longer range wireless
- Compare speed/cost: dial-up (cheapest/slowest) → broadband → leased line (costliest/most reliable)

### Unit 4: Electronic Mail Systems

#### 4.4.1 Electronic Mail — Address, Components, and Protocols 🔥

**Theory**

**Email** transmits messages between computers via Internet — one of the most used Internet services. Messages may contain text, images, audio, or attachments. Address format: `username@domainname` (e.g., sachin@gmail.com) — not case-sensitive, no spaces. Email systems use standard **protocols** for sending and receiving: **SMTP** (send), **POP3** and **IMAP** (receive).

**Important Points**

| Component | Function |
|-----------|----------|
| User Agent (UA) | Program to compose, send, receive, reply to messages (Outlook, Thunderbird) |
| Message Transfer Agent (MTA) | Transfers email between systems using SMTP; client MTA + system MTA |
| Mailbox | File on local hard drive collecting delivered emails |
| Spool file | Contains outgoing emails; MTA extracts for delivery |

| Protocol | Full Form | Purpose | Port | Key Trait |
|----------|-----------|---------|------|-----------|
| SMTP | Simple Mail Transfer Protocol | **Sending** email between servers | 25/587 | MTA uses SMTP to push mail to recipient server |
| POP3 | Post Office Protocol v3 | **Receiving** email; downloads to local device | 110/995 | Mail removed/stored locally; offline access |
| IMAP | Internet Message Access Protocol | **Receiving** email; syncs with server | 143/993 | Mail stays on server; access from multiple devices |

- Email services provided by system:

| Service | Description |
|---------|-------------|
| Composition | Creating messages and replies |
| Transfer | Sending email from sender to recipient |
| Reporting | Confirming delivery, loss, or rejection |
| Displaying | Presenting email in readable format |
| Disposition | Save, delete before/after reading |

- **SMTP** = outbound; MTA uses SMTP to push mail to recipient server via spool file
- **POP3** downloads messages to local mailbox; good for single-device offline reading
- **IMAP** keeps messages on server; folders synced across phone, laptop, tablet
- Email services: Composition, Transfer, Reporting, Displaying, Disposition
- Sender and recipient both need valid `username@domainname` addresses

**For Exam**

Email transfers messages via Internet using `username@domainname` addresses. Components: User Agent (compose/send/receive), MTA (transfers between systems via SMTP), Mailbox (incoming storage), Spool file (outgoing queue). Protocols: SMTP sends mail between servers; POP3 receives and downloads mail locally; IMAP receives while keeping mail on server for multi-device sync. Services include composition, transfer, delivery reporting, display, and disposition.

#### 4.4.2 Email Software Features

**Theory**

Email software provides sending, receiving, filtering, attaching, forwarding, CC, and BCC features. Two types: **email clients** (Outlook — manual send/receive, auto-download attachments) and **webmail** (Gmail, Yahoo — refresh page, manual attachment download).

**Important Points**

- **CC (Carbon Copy):** all CC recipients visible to each other; like carbon paper between sheets
- **BCC (Blind Carbon Copy):** only sender sees BCC list; recipients unaware of each other
- **Filtering:** routes mail to folders at server; suspicious → spam/junk; blocks malicious links/code
- **Attach steps:** Compose → Attach Files → Choose File → Open → Send
- **Forward:** select message → enter destination → use forward symbol (no recomposition needed)
- Email clients (Outlook): click Send/Receive; attachments auto-download
- Webmail (Gmail, Yahoo): refresh page; manually download attachments
- Send steps: login → Compose/New → To + Subject + Body → Send

**For Exam**

Email features include send, receive, filter, attach, forward, CC, and BCC. Email clients (Outlook) run on the computer — click Send/Receive, attachments auto-download. Webmail (Gmail, Yahoo) runs in browser — refresh to check, manually download attachments. CC (Carbon Copy) shows all recipients to each other; BCC (Blind Carbon Copy) hides recipients from one another. Filtering routes mail to folders at the server; suspicious mail goes to spam. Attach: Compose → Attach Files → Choose File → Send. Forward resends a received message without recomposition.

#### 4.4.3 Web-Based Systems

**Theory**

**Web-based systems** use web applications over Internet to accomplish tasks (Google Meet, Zoom, online forms, shopping carts). Web applications are coded in JavaScript and HTML, executed via browser. Dynamic apps need server-side processing; static apps do not.

**Important Points**

- Working (5 steps): browser requests app → Internet forwards to web app server → server processes → returns page via Internet → displays on user screen
- Architecture: web server (receives requests) + application server (processes tasks) + database (stores data)
- Dynamic apps need server-side processing; static apps run entirely in browser
- Benefits: **Data Recovery**, **Better Security**, **Competitive Edge**, **Improved Efficiency**, **Greater Visibility**, **24/7 Accessibility**
- Integratable features: **Mobile Interface**, **Social Integration**, **Analytics**, **Live Chat**, **Web Payments**
- Examples: Google Meet, Zoom, Google Apps, Microsoft 365, online forms, shopping carts

**For Exam**

Web-based systems use web applications (JavaScript, HTML) via browsers to accomplish Internet tasks like Google Meet, Zoom, and online shopping. Architecture: browser → Internet → web application server → database. Five-step flow: request → forward to server → process → return page → display. Benefits: data recovery, security, competitive edge, efficiency, visibility, 24/7 access. Integratable features: mobile interface (desktop + phone), social integration (quick registration), analytics (user insights), live chat (customer support), web payments (one-step checkout).

#### 4.4.4 Web Pages

**Theory**

A **web page** displays text, figures, audio, video, animations, and links in a browser. Collection of linked pages = **website**. Pages classify as **static** (fixed content, stored as-is) or **dynamic** (content changes without full reload, per-user variation).

**Important Points**

| Page Type | Purpose | Example Use |
|-----------|---------|-------------|
| Home Page | Starting point; website introduction and navigation | www.sgou.ac.in landing tab |
| Feed Page | Updates content dynamically | Social media following updates |
| Menu Page | Navigation to content categories | Restaurant-style content list |
| Search Page | Internal search to jump to results | Site search field |
| About Page | Company/product/person info; branding | Administration, Academics tabs |
| Registration Page | Create/login to personalised accounts | Facebook, email signup |
| 404 Page | Error — page not found or broken link | Deleted/dead link response |
| Portfolio Page | Professional visual presentation | Designs, art, handmade goods |
| Product Page | E-commerce details, reviews, cart/wishlist | Amazon smartphone listing |

- Static page: content loaded exactly as stored on server; created with HTML
- Dynamic page: portion changes without full reload; HTML + JavaScript; per-user content
- Each page has unique URL; collection of linked pages = website on web server

**For Exam**

Web pages are browser documents displaying text, figures, audio, video, animations, and links — like encyclopaedia pages on web servers. Static pages load exactly as stored (HTML); dynamic pages change portions without full reload (HTML + JavaScript). Nine page types: Home (starting point), Feed (content updates), Menu (navigation list), Search (internal results), About (branding info), Registration (account login), 404 (not found error), Portfolio (visual showcase), Product (e-commerce with reviews/cart). Each page has a unique URL; linked pages form a website.

### Unit Recap (from SLM)
- **Email** transfers messages; needs sender/recipient addresses (username@domain)
- Components: **UA**, **MTA**, **Mailbox**, **Spool file**
- Protocols: **SMTP** (send), **POP3** (download receive), **IMAP** (server-sync receive)
- Email types: **clients** (Outlook) and **webmail** (Gmail)
- Features: send, receive, filter, attach, forward, **CC**, **BCC**
- **Web-based systems** use web applications (JavaScript, HTML)
- Web pages: **Static** (fixed) and **Dynamic** (changing)
- Page types: Home, Feed, Menu, Search, About, Registration, 404, Portfolio, Product


## Block 5: Hypertext Markup Language

**Course Code:** B21CA01DC | **Programme:** BCA | **University:** SGOU  
**Coverage:** Block 5 — Units 1–4 (HTML) | **Source:** SGOU SLM B21CA01DC

### Unit 1: HTML — Basic Tags and Divisions

#### 5.1.1 HTML Structure, Document Types and Rules 🔥

**Theory**

A **website** is a collection of web pages accessible through the Internet; each page is built with **HTML** (Hypertext + Markup Language). Hypertext links documents; markup tags define structure. **CSS** handles presentation; **JavaScript** adds interactivity. **HTML5** is the latest version (video streaming, location support). An **HTML element** has opening tag, content, and closing tag; syntax is `<tagname> Content </tagname>`. Tags are **paired** (opening + closing) or **singular/empty** (e.g. `<br>`). Attributes in the opening tag use `name="value"` in quotation marks.

The document structure (Fig 5.1.2): `<!DOCTYPE html>` → `<html>` (root) → `<head>` (metadata, not visible) → `<title>` (browser title bar) → `<body>` (visible content). Save as `.html` or `.htm` using Notepad/TextEdit; browser renders the file top-to-bottom, left-to-right. HTML versions evolved from 1.0 (basic text/images) through 2.0, 3.0 (CSS support), 4.1 (external CSS) to HTML5.

**HTML document types:** (1) **Transitional** — most used, flexible syntax, browsers use "best effort" without reporting errors; (2) **Strict** — enforces rules, all opened tags need closing tags, faster on mobile; (3) **Frameset** — multiple documents on one screen (menu systems).

| Version | Year | Key Features |
|---------|------|-------------|
| HTML 1.0 | 1991 | Basic text controls and images only |
| HTML 2.0 | — | Common rules; text boxes, buttons |
| HTML 3.0 | — | Improved tags; CSS support |
| HTML 4.1 | — | External CSS file inclusion |
| **HTML5** | Current | Video streaming, location support, modern APIs |

**HTML rules:** sketch layout on paper first; tags in angle brackets `<tag>`; opening on / closing off (`<BR>` exception); closing uses forward slash `</tag>`; nested tags closed inner-first; optional attributes modify behaviour (e.g. `<P ALIGN=CENTER>`). Older browsers ignore unknown tags without breaking recognised content.

**Important Points**

- HTML = Hypertext (links) + Markup Language (tags); invented 1991 by Tim Berners-Lee
- HTML versions: 1.0 → 2.0 → 3.0 → 4.1 → **HTML5**
- DOCTYPE on first line tells browser the HTML version
- `<title>` = browser tab title; `<h1>` = page content heading (different purposes)
- Three document types: Transitional, Strict, Frameset
- Five coding rules: angle brackets, on/off switch, forward slash, correct nesting, attributes
- Paired tags have opening and closing; singular/empty tags (br, img, meta) need no closing
- Attribute values must always be enclosed in quotation marks
- Design on paper before coding to avoid rework with HTML tags

**Common Global Attributes (apply to most HTML elements):**

| Attribute | Example | Purpose |
|-----------|---------|---------|
| **id** | `id="section1"` | Unique identifier; target for internal links |
| **class** | `class="header-box"` | Groups elements for CSS styling |
| **style** | `style="color:red;"` | Inline CSS styling on any element |
| **title** | `title="Tooltip text"` | Tooltip shown on mouse hover |
| **lang** | `<html lang="en">` | Declares document language |

**For Exam**

HTML is a structured markup language combining hypertext links and tags to define web page structure. A basic document contains DOCTYPE, html, head (title, meta, link, style), and body. Documents are classified as Transitional (flexible), Strict (rule-enforced), or Frameset (multiple frames). Key rules: tags in angle brackets, paired tags with forward-slash closing, correct nesting, and attributes in quotes. HTML5 is the current standard supporting multimedia and modern web features. Tim Berners-Lee invented HTML in 1991; each HTML file is plain text with a .html extension read by browsers top-to-bottom.

```html
<!DOCTYPE html>
<html>
<head><title>Web Page</title></head>
<body>
<h1>Distance Learning Computer Science</h1>
<p>A portal for Students</p>
</body>
</html>
```

#### 5.1.4–5.1.9 HTML Tags — Head, Body, Headings, Div and Center 🔥

**Theory**

**HTML tags** are keywords helping browsers format content; each tag has opening tag, content, and closing tag (some have no closing). The **head tag** (`<head>`) holds metadata — title, character set, styles, links, scripts — not displayed on the page. Head elements: **title** (one per document, browser title bar), **style** (inline CSS in head), **base** (absolute URL, one only, empty tag), **link** (external CSS via `rel` and `href`, empty tag), **meta** (keywords, description, viewport for search engines, empty tag).

The **body tag** defines visible content (text, images, links); placed inside `<html>` after `<head>`; only one body per document. **Headings** `<h1>`–`<h6>`: h1 = most important, h6 = least; help search engines index structure. **Division tag** `<div>` groups elements for CSS styling; block-level, no layout effect alone. **Center tag** `<center>` aligns text, graphics, and tables to centre. Browsers read HTML top-to-bottom and distinguish tagged content from plain text.

| Head Element | Syntax Example | Purpose |
|--------------|---------------|---------|
| **title** | `<title>Page Title</title>` | Browser title bar; one per document |
| **style** | `<style>h1{color:#1c87c9}</style>` | Inline CSS styling inside head |
| **base** | `<base href="https://site.com/" target="_blank">` | Absolute base URL; one only; empty tag |
| **link** | `<link rel="stylesheet" href="style.css">` | Links external CSS file; empty tag |
| **meta** | `<meta name="keywords" content="HTML, CSS">` | Keywords, description, viewport; empty tag |
| **meta viewport** | `<meta name="viewport" content="width=device-width, initial-scale=1.0">` | Responsive design on all devices |

| Body Tag | Syntax Example | Purpose |
|----------|---------------|---------|
| **h1–h6** | `<h1>Main Heading</h1>` | Six heading levels by importance |
| **div** | `<div>Grouped content</div>` | Block-level container for CSS grouping |
| **center** | `<center>Centred text</center>` | Aligns text, graphics, tables to centre |
| **p** | `<p>Paragraph text</p>` | Paragraph of text |
| **body** | `<body>Visible content</body>` | All visible page content; one per document |

**Important Points**

- Head metadata: title, style, base, link, meta — invisible to user
- Title tag ≠ h1: title = entire document title in browser bar; h1 = page heading
- Link tag: `<link rel="stylesheet" href="style.css">` loads external CSS
- Meta viewport: `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
- Six heading levels: h1 (largest/most important) to h6 (smallest)
- `<div>` = container for grouping; `<center>` = centre alignment
- Base tag sets default URL for all relative links on the page
- Meta description helps search engines index the page content
- Only one `<title>` and one `<base>` tag allowed per document

**For Exam**

HTML tags format browser display. The head section contains metadata elements: title (browser title bar, one only), style (CSS in head), base (absolute URL), link (external resources), and meta (keywords, description, viewport). The body tag holds all visible content. Six heading levels (h1–h6) structure content by importance. The div tag groups elements for CSS styling as a block-level container. The center tag aligns content to the centre of the page. Title tag content appears in the browser title bar but not on the page itself, whereas h1 appears as visible page content. Meta keywords and description help search engines index the page; meta viewport ensures responsive display on mobile devices.

### Unit Recap — Unit 1

- HTML = Hypertext + Markup Language; HTML5 is the latest version
- CSS = presentation; JavaScript = interactivity
- Element syntax: `<tagname> Content </tagname>`; attributes in opening tag
- Document structure: DOCTYPE → html → head → title → body
- Document types: Transitional (flexible), Strict (enforced), Frameset (frames)
- Head elements: title, style, base, link, meta
- Body = visible content; h1–h6 headings; div = grouping; center = alignment

### Unit 2: Managing List and Table

#### 5.2.1 HTML Lists 🔥

**Theory**

HTML **lists** present information in a well-formed, semantic manner. Three types: **Unordered list** (`<ul>`) — items with no numerical order, shown as bullets; each item uses `<li>`. **Ordered list** (`<ol>`) — items numbered 1, 2, 3…; each item uses `<li>`. **Description list** (`<dl>`) — terms with descriptions like a dictionary; **dt** = term, **dd** = description (at least one dt followed by one dd per group). Lists help organise content the way a programme coordinator arranges festival events. All three list types use paired opening/closing tags.

| List Type | Opening Tag | Item Tag | Description Tag | Display Style |
|-----------|------------|----------|-----------------|---------------|
| Unordered | `<ul>` | `<li>` | — | Bullet points |
| Ordered | `<ol>` | `<li>` | — | Numbers 1, 2, 3… |
| Description | `<dl>` | — | `<dt>` + `<dd>` | Term + description pairs |

**Important Points**

- Unordered: `<ul><li>item</li></ul>` — bullet points
- Ordered: `<ol><li>item</li></ol>` — numbered list
- Description: `<dl><dt>term</dt><dd>desc</dd></dl>`
- `<li>` must be inside ul, ol, or menu parent
- Lists introduce information semantically
- Changing order in unordered list does not change meaning
- Each element in unordered/ordered list declared inside parent tag
- Description list arranged like a dictionary with terms and meanings

**For Exam**

HTML provides three list types. Unordered lists (`<ul>`) group items without numerical order using bullet points; each item is an `<li>` element. Ordered lists (`<ol>`) number items sequentially starting 1, 2, 3. Description lists (`<dl>`) pair terms (`<dt>`) with descriptions (`<dd>`), similar to a dictionary. The `<li>` tag represents an individual list item within its parent list. All three list types come in paired opening/closing tags. Changing the order of items in an unordered list does not change the meaning, whereas order matters in ordered lists.

#### 5.2.2 HTML Tables 🔥

**Theory**

HTML **tables** create rows and columns on a web page using `<table>`, `<tr>` (table row), `<td>` (standard data cell), and `<th>` (header cell). All tr tags are declared inside table. td/th are child elements of tr. Table size adjusts to content. **colspan** spans cells across columns; **rowspan** spans across rows. Tables are analogous to inserting a table in Microsoft Word using rows and columns.

| Tag | Attribute Examples | Purpose |
|-----|-------------------|---------|
| **table** | `<table border="1" width="80%">` | Defines the table container |
| **tr** | `<tr align="center">` | Defines a row inside table |
| **td** | `<td colspan="2">Merged cell</td>` | Standard data cell; left-aligned default |
| **th** | `<th rowspan="2">Header</th>` | Header cell; bold/centred by default |
| **colspan** | `colspan="2"` | Merges cell across 2 columns |
| **rowspan** | `rowspan="3"` | Merges cell across 3 rows |

**Important Points**

- Structure: `<table>` → `<tr>` → `<td>` or `<th>`
- `<th>` = header cell (bold/centred by default)
- `<td>` = data cell (left-aligned by default)
- colspan and rowspan control cell spanning
- tr must be inside table tag
- Tables organise tabular data on web pages
- td and th can contain text, images, and other HTML content
- Table size automatically adjusts based on content size

**Example table with colspan:**

```html
<table>
<tr><th>Name</th><th colspan="2">Contact</th></tr>
<tr><td>Ali</td><td>Email</td><td>Phone</td></tr>
</table>
```

**For Exam**

HTML tables are built with the table tag containing rows (`<tr>`), which contain data cells (`<td>`) or header cells (`<th>`). Header cells label columns or rows and appear bold/centred by default; data cells hold content and are left-aligned. The colspan attribute merges cells horizontally across columns; rowspan merges vertically across rows. All tr tags must be declared inside the table tag. Tables provide structured display of tabular information on web pages, similar to tables in Microsoft Word.

#### 5.2.3 HTML Frames 🔥

**Theory**

An HTML **frame** defines a window loading another web page; uses **src** attribute for URL; empty tag (no closing). **Frameset** divides the browser window into frames using **rows** (horizontal) or **cols** (vertical) attributes. Frameset comes in pairs; can contain one or more frame tags and nest framesets for smaller divisions. Used for menu systems where one section reloads while menu stays fixed. Clicking a menu item reloads only the content frame, not the entire page. Percentage values in cols/rows (e.g. `cols="50%,50%"`) define proportional frame sizes.

| Tag | Attribute Examples | Purpose |
|-----|-------------------|---------|
| **frameset** | `<frameset cols="50%,50%">` | Divides window into vertical frames |
| **frameset** | `<frameset rows="30%,70%">` | Divides window into horizontal frames |
| **frame** | `<frame src="page.html">` | Loads external page; empty/singular tag |
| **src** | `src="https://example.com"` | URL of the web page to load in frame |

**Important Points**

- `<frame src="url">` — empty/singular tag
- `<frameset cols="50%,50%">` divides window vertically
- `<frameset rows="...">` divides horizontally
- Frameset can nest for complex layouts
- Frame tag used with frameset element
- Common use: fixed menu + changing content area
- src attribute defines address of web page in frame
- Nested framesets divide windows into smaller sections

**For Exam**

HTML frames display multiple web pages in one browser window. The frameset tag divides the window using rows or cols attributes and contains frame tags. Each frame tag loads an external page via the src attribute. Framesets can be nested for complex layouts. This technique is commonly used for menu systems where navigation remains static while content reloads. The frame tag is empty (no closing tag) and must be used inside a frameset element. Percentage values in cols/rows define proportional frame sizes.

```html
<!DOCTYPE html>
<html>
<head><title>Lists Example</title></head>
<body>
<h1>Unordered List</h1>
<ul><li>Item 1</li><li>Item 2</li></ul>
<h1>Ordered List</h1>
<ol><li>First</li><li>Second</li></ol>
</body>
</html>
```

### Unit Recap — Unit 2

- Three list types: unordered (ul), ordered (ol), description (dl/dt/dd)
- `<li>` represents a list item inside ul or ol
- Tables: table → tr → td/th
- colspan and rowspan span multiple columns/rows
- Frame tag loads external pages; frameset divides window
- rows = horizontal frames; cols = vertical frames

### Unit 3: Presenting Multimedia

#### 5.3.1–5.3.2 Image Tag and HTML Colors 🔥

**Theory**

**Multimedia** is an interactive mass communication medium (text, graphics, audio, video, animation). The **image tag** `<img>` embeds images; image is not inserted directly — browser loads from source. Required attributes: **src** (image URL) and **alt** (alternate text). Also specify **width** and **height** to prevent flicker. Empty tag — no closing tag. Image formats include JPEG, PNG, GIF, BMP, TIFF.

**HTML colors** three methods: (1) **Hex codes** — six-digit number with `#` (e.g. `#FF0000` = red; min `#000000`, max `#FFFFFF`); (2) **Color names** (e.g. `blue`, `white`); (3) **RGB values** — `rgb(255,0,0)`; values 0–255 per channel; black = `rgb(0,0,0)`, white = `rgb(255,255,255)`. Hex uses base-16 (0–9, A–F); letters not case-sensitive.

| Tag/Method | Attribute / Syntax | Example | Purpose |
|------------|-------------------|---------|---------|
| **img** | `src` | `src="/images/photo.jpg"` | Image file URL (required) |
| **img** | `alt` | `alt="Baby Photo"` | Alternate text if image fails (required) |
| **img** | `width`, `height` | `width="200" height="185"` | Prevents page flicker while loading |
| **Hex color** | `#RRGGBB` | `#FF0000` = red; `#0000FF` = blue | Six-digit hex colour code |
| **Color name** | name | `background-color: blue` | Named colour in CSS/style |
| **RGB** | `rgb(R,G,B)` | `rgb(255,0,0)` = red | Red/Green/Blue 0–255 each |

| Colour | Hex Value | RGB Value |
|--------|-----------|-----------|
| Black | `#000000` | `rgb(0,0,0)` |
| White | `#FFFFFF` | `rgb(255,255,255)` |
| Red | `#FF0000` | `rgb(255,0,0)` |
| Blue | `#0000FF` | `rgb(0,0,255)` |
| Cyan | `#00FFFF` | `rgb(0,255,255)` |
| Magenta | `#FF00FF` | `rgb(255,0,255)` |

**Important Points**

- `<img src="url" alt="text" width="200" height="185">`
- Image formats: JPEG, PNG, GIF, BMP, TIFF
- Hex: base-16; 6 digits after `#`; not case-sensitive
- RGB: red, green, blue each 0–255
- style attribute adds colour to elements
- Multimedia elements: text, image, audio, video, animation
- src and alt are the two required attributes of img tag
- Minimum hex/RGB = black; maximum = white

**For Exam**

The img tag inserts images using src (URL) and alt (alternate text) attributes; width and height prevent layout flicker while the image loads. Colours are specified three ways: hexadecimal codes (#RRGGBB, six digits starting with #), HTML colour names (blue, red, white), or RGB values rgb(R,G,B) with each component 0–255. Hex black is #000000 and white is #FFFFFF; RGB black is rgb(0,0,0) and white is rgb(255,255,255). Hex uses base-16 (0–9, A–F). The img tag is empty — no closing tag required. Image formats include JPEG, PNG, GIF, BMP, and TIFF.

#### 5.3.3–5.3.4 Marquee and Multimedia Tags 🔥

**Theory**

The **marquee tag** scrolls text or images horizontally or vertically: `<marquee> content </marquee>`. **Multimedia tags** embed audio/video: **audio** — plays audio files; uses src or `<source>`; **controls** adds play/pause/volume; formats MP3, WAV. **video** — displays video; formats MP4/MPEG-4, WebM; attributes: controls, muted, width, height. **source** — defines multiple media formats (empty tag). **embed** — container for external applications/plugins (empty tag). **object** — embeds multimedia or another HTML document (paired tag). Browser chooses supported format from source tag options.

| Tag | Key Attributes | Example | Purpose |
|-----|---------------|---------|---------|
| **marquee** | direction, behaviour | `<marquee>Scrolling text</marquee>` | Scrolls text/image horizontally or vertically |
| **audio** | controls, src | `<audio controls src="song.mp3">` | Embeds audio; MP3, WAV formats |
| **source** | src, type | `<source src="file.mp3" type="audio/mpeg">` | Multiple format fallback; empty tag |
| **video** | controls, muted, width, height | `<video controls width="300">` | Embeds video; MP4, WebM formats |
| **embed** | type, src, width, height | `<embed type="audio/mpeg" src="audio.mp3">` | External plugin content; empty tag |
| **object** | width, height, data | `<object data="video.swf">` | Embedded object/document; paired tag |

**Important Points**

- Marquee: paired tag; scrolls text left-right or top-bottom
- Audio: `<audio controls><source src="file.mp3" type="audio/mpeg"></audio>`
- Video: `<video controls src="file.mp4"></video>`
- source tag enables multiple format fallbacks
- embed = external plugin content (no closing tag)
- object = embedded object with opening/closing tags
- controls attribute adds play, pause, and volume buttons
- muted attribute silences video on load

**For Exam**

The marquee tag creates scrolling text or images on a web page horizontally or vertically. Multimedia is embedded using audio tag (plays audio with controls and source), video tag (displays video with controls, muted, width, height), embed tag (external plugin content, empty tag), and object tag (embedded objects/documents, paired tag). The source tag specifies alternative media formats so browsers choose supported formats. Supported audio formats include MP3 and WAV; video formats include MP4/MPEG-4 and WebM. The controls attribute adds play, pause, and volume buttons to audio and video players.

```html
<!DOCTYPE html>
<html>
<head><title>Multimedia</title></head>
<body>
<img src="photo.jpg" alt="Photo" width="200" height="185"/>
<audio controls>
<source src="song.mp3" type="audio/mpeg">
</audio>
</body>
</html>
```

### Unit Recap — Unit 3

- Multimedia = interactive digital medium (text, image, audio, video)
- img: src + alt required; empty tag
- Colours: hex (#RRGGBB), names, RGB rgb(0–255)
- Marquee scrolls text/images
- audio, video, embed, object = multimedia tags
- source defines multiple media formats

### Unit 4: Linking in HTML

#### 5.4.1–5.4.4 HTML Links, Anchor, Internal and External Linking 🔥

**Theory**

An HTML **hyperlink** connects one web page to another; has two ends — **anchor** (text marking start/end) and **direction**. Link starts at source anchor, ends at destination anchor. Created with **anchor tag** `<a href="URL">content</a>`. Default colours: **unvisited = blue**, **visited = purple**, **active = red** (all underlined). Links apply to text, images, and other elements. Hyperlinks can connect to HTML documents, images, video, audio, or elements within a document.

**Internal linking** — links within same page using **hash (#)** and **id**: `<a href="#section1">Go</a>` … `<a id="section1">Section</a>`. Path may be absolute or relative. **External linking** — connects to other web pages via href URL; no hash symbol needed. Example: `<a href="https://example.com">Visit</a>`. Relative paths like `../tutorial.php` navigate within site structure.

| Tag/Concept | Attribute / Syntax | Example | Purpose |
|-------------|-------------------|---------|---------|
| **a (anchor)** | `href` | `<a href="https://flipkart.com">Shop</a>` | Creates hyperlink to URL |
| **a (internal)** | `href="#id"` | `<a href="#lesson1">Lesson 1</a>` | Scrolls to section on same page |
| **a (external)** | `href="url"` | `<a href="../css/page.php">CSS</a>` | Links to external/relative page |
| **id** | `id="name"` | `<a id="lesson1">Introduction</a>` | Target anchor for internal links |
| **linked image** | a + img | `<a href="url"><img src="pic.jpg"></a>` | Image acts as clickable link |

| Link State | Default Colour | Description |
|------------|---------------|-------------|
| Unvisited | Blue (underlined) | Link not yet clicked |
| Visited | Purple (underlined) | Link previously clicked |
| Active | Red (underlined) | Link currently being clicked |

**Important Points**

- Anchor tag: `<a href="url">text</a>` — paired tag
- href attribute = destination URL
- Internal: `#id` scrolls to section on same page
- External: full or relative URL to other pages
- Default link colours: blue (unvisited), purple (visited), red (active)
- Images as links: `<a href="url"><img src="..." alt=""></a>`
- Source anchor = where link starts; destination anchor = where it ends
- Absolute path = full original URL; relative path = path within site

**For Exam**

HTML hyperlinks connect pages using the anchor tag with href attribute. A link has source anchor (where it starts) and destination anchor (where it ends). Default colours: blue (unvisited), purple (visited), red (active) — all underlined. Internal links use hash (#) with id attributes to scroll to sections on the same page. External links use href with absolute URLs (full web address) or relative URLs (path within site). Hyperlinks can be applied to text, images, and other HTML elements. Clicking a linked image redirects to the href URL.

#### 5.4.5 Creating a Website 🔥

**Theory**

Creating a website requires **HTML** (structure/content) and **CSS** (styling/presentation). Prerequisites: web hosting service and unique domain name (e.g. www.example.org). **Eleven steps:** (1) Study HTML basics; (2) Learn document structure; (3) Save as .html/.htm (UTF-8 encoding); (4) Learn CSS selectors (e.g. `p { font-size: 18px; }`); (5) Combine CSS documents in order; (6) Install **Bootstrap** (open-source HTML/CSS framework); (7) Pick a design/template; (8) Customize with HTML and CSS; (9) Add content and images; (10) Fine-tune colours and fonts; (11) Create additional pages (about, contact, portfolio, products, team, policies) and link to homepage. Sublime Text editor provides syntax colour highlighting for easier coding.

**Important Points**

- HTML = structure; CSS = presentation; Bootstrap = responsive framework
- Save HTML with .html extension; UTF-8 encoding preferred
- CSS class selector: `.classname { property: value; }`
- Bootstrap provides pre-built templates and grid system
- Additional pages: about, contact, portfolio, services, policies
- Upload .html files to web server main directory
- CSS tag selector: `p { font-size: 18px; }` styles all paragraph tags
- Bootstrap viewport meta tag: `width=device-width, initial-scale=1`
- Copy .html file to web server directory to publish online

**Eleven Website Creation Steps (Detailed):**

| Step | Action | Detail |
|------|--------|--------|
| 1 | Study HTML basics | Recall tags: `<i>`, `<p>`, `<ul>`, headings from previous units |
| 2 | Learn document structure | DOCTYPE → html → head → title → body |
| 3 | Save HTML document | Notepad/TextEdit; save as index.html; UTF-8 encoding |
| 4 | Learn CSS selectors | Tag selector `p{}` and class selector `.name{}` |
| 5 | Combine CSS documents | Arrange CSS in order matching HTML structure |
| 6 | Install Bootstrap | Open-source framework; download from getbootstrap.com |
| 7 | Pick a design | Choose Bootstrap template; copy to web server directory |
| 8 | Customize with HTML/CSS | Edit homepage head section, meta viewport, link CSS |
| 9 | Add content and images | Use header, footer, section tags; assign CSS classes |
| 10 | Fine-tune colours/fonts | Hex values e.g. `#FF0000` for red text via style attribute |
| 11 | Create additional pages | About, contact, portfolio, products, team, policies — link all to homepage |

**For Exam**

Website creation combines HTML for structure and CSS for styling. Steps include learning HTML/CSS, saving documents as .html files with UTF-8 encoding, selecting CSS selectors (tag and class), installing Bootstrap framework, choosing a template, customizing design, adding content/images, fine-tuning colours/fonts, and creating linked additional pages. Prerequisites include web hosting (space on web server) and a domain name (unique website identifier). Bootstrap is open-source software providing templates and responsive design tools. Sublime Text editor provides syntax highlighting for easier HTML coding.

```html
<!DOCTYPE html>
<html>
<head><title>Links</title></head>
<body>
<a href="https://www.example.com">External Link</a>
<a href="#top">Internal Link</a>
<a id="top">Section Top</a>
</body>
</html>
```

### Unit Recap — Unit 4

- Hyperlink connects pages; anchor tag + href attribute
- Link colours: blue (unvisited), purple (visited), red (active)
- Internal links: #id on same page
- External links: URL to other pages
- Website needs hosting + domain name
- Bootstrap + HTML + CSS for website creation

### HTML Quick Reference — Key Attributes Summary

| Tag | Key Attributes | Example Usage |
|-----|---------------|---------------|
| `<html>` | lang | `<html lang="en">` — root element |
| `<head>` | — | Contains metadata; not visible on page |
| `<title>` | — | `<title>Page Title</title>` — browser tab |
| `<meta>` | name, content | `<meta name="description" content="About page">` |
| `<link>` | rel, href, type | `<link rel="stylesheet" href="style.css">` |
| `<body>` | bgcolor, background | Contains all visible page content |
| `<h1>`–`<h6>` | align | `<h1 align="center">Heading</h1>` |
| `<p>` | align | `<p align="center">Centred paragraph</p>` |
| `<div>` | id, class, style | `<div id="main" class="box">` — grouping |
| `<ul>` / `<ol>` | type, start | `<ol start="5">` — ordered from 5 |
| `<li>` | value | `<li value="3">Third item</li>` |
| `<table>` | border, width, cellpadding | `<table border="1" width="100%">` |
| `<tr>` | align, valign | Row inside table |
| `<td>` | colspan, rowspan, align | `<td colspan="2">Merged</td>` |
| `<th>` | colspan, rowspan, scope | Header cell; bold by default |
| `<img>` | src, alt, width, height | `<img src="pic.jpg" alt="Photo">` |
| `<a>` | href, target, id | `<a href="#top" target="_blank">` |
| `<audio>` | controls, src, autoplay | `<audio controls src="song.mp3">` |
| `<video>` | controls, width, height, muted | `<video controls width="300">` |
| `<source>` | src, type | `<source src="file.mp3" type="audio/mpeg">` |
| `<marquee>` | direction, behaviour | `<marquee direction="left">Text</marquee>` |
| `<frameset>` | rows, cols | `<frameset cols="50%,50%">` |
| `<frame>` | src, name, noresize | `<frame src="page.html">` — empty tag |
| `<embed>` | type, src, width, height | External plugin content |
| `<object>` | width, height, data | Embedded object; paired tag |


## Block 6: Trends in Information Technology

**Course Code:** B21CA01DC | **Coverage:** Block 6 — Units 1–4 | **Source:** SGOU SLM B21CA01DC

### Unit 1: Applications of IT

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

#### 6.1.2 IT in Business

**Theory**

IT supports business through: **Organisational Communication** — email, Google Meet, virtual meetings worldwide. **Inventory Management** — software tracks stock levels, monitors and reorders automatically. **E-commerce** — online buying/selling of goods and services via social media and shopping websites; saves time, labour, advertising costs. **CRM (Customer Relationship Management)** — tracks purchases, provides 24/7 customer service online. **Decision-Making** — decision support systems show real-time performance (capital, sales, trends) for promotion/expense decisions. **Internet Enabled Systems** — improve security; e.g. CCTV reduces theft and data loss. Employees can share work reports regardless of location.

| Business IT Application | Tool / Method | Benefit |
|------------------------|--------------|---------|
| Communication | Email, Google Meet | Virtual meetings across locations |
| Inventory Management | Inventory software | Auto stock tracking and reordering |
| E-commerce | Facebook, WhatsApp, shopping sites | Saves time, labour, advertising cost |
| CRM | CRM systems | 24/7 customer service; tracks purchases |
| Decision-Making | Decision support systems | Real-time performance monitoring |
| Security | CCTV, Internet Enabled Systems | Reduces theft and data loss |

**Important Points**

- Communication: email, video conferencing for virtual meetings
- Inventory Management software tracks stock and auto-reorders
- E-commerce = online buying/selling; saves costs
- CRM improves customer experience 24/7
- Decision support systems enable real-time performance monitoring
- Internet Enabled Systems (CCTV) improve business security
- CRM tracks customer purchases and assists via website/social media
- E-commerce uses Facebook, WhatsApp, YouTube, and shopping websites

**For Exam**

IT plays a vital role in business through organisational communication (email, Google Meet, virtual meetings with staff/clients worldwide), inventory management software (tracks stock, auto-reorders raw materials), e-commerce (online buying/selling via Facebook, WhatsApp, shopping websites — saves time, labour, advertising costs), CRM systems (tracks customer purchases, provides 24/7 service after business hours), decision support systems (real-time monitoring of capital, sales, marketing trends for promotion decisions), and internet-enabled security systems like CCTV (reduces theft and confidential data loss).

#### 6.1.3 IT in Banking — Electronic Services ⭐

**Theory**

IT revolutionised banking enabling **Any Time, Any Where Banking**. Multiple electronic mechanisms connect bank branches and customers digitally. **ECS** handles bulk salary payments to many accounts. **MICR** uses magnetic ink for electronic cheque clearing with a **9-digit code** (3 city + 3 bank + 3 branch digits). **NEFT** is RBI-maintained nationwide transfer in batches (not instant). **RTGS** settles funds in real time — the fastest channel. **CBS** networks all branches for any-branch banking. **ATM** dispenses cash via magnetic strip cards. Tele banking provides 24-hour voice service; internet banking via website; mobile banking via installed app.

**Important Points**

- ECS = bulk electronic fund transfer between accounts
- MICR = 9-digit code for electronic cheque clearing
- NEFT = RBI nationwide one-to-one transfer (batch, not real-time)
- RTGS = real-time gross settlement; fastest banking channel
- CBS = all branches networked; any-branch banking
- ATM = cash dispensing; magnetic strip cards
- NEFT requires beneficiary addition before transfer
- RTGS has no waiting period — processed immediately

**For Exam**

IT in banking includes multiple electronic services enabling Any Time, Any Where Banking. ECS handles bulk salary/fund transfers (one-to-many). MICR electronically clears cheques using 9-digit magnetic ink codes (3 city + 3 bank + 3 branch). NEFT (RBI-maintained) transfers funds one-to-one between NEFT-enabled accounts in batches — add beneficiary first via Internet banking. RTGS settles in real time without delay — the fastest banking channel for high-value transfers. CBS networks all branches for any-branch operations via centralized data. ATMs dispense cash using debit/credit card magnetic strips. Tele banking (24-hour voice), Internet banking (website + username/password), and Mobile banking (installed app) extend round-the-clock access.

| Service | Full Form | Timing / Settlement | Key Features |
|---------|-----------|--------------------|-|
| **ECS** | Electronic Clearing Services | Batch processing | Bulk transfer: one account to many or vice versa; used for salary payments |
| **MICR** | Magnetic Ink Character Recognition | Cheque clearing | 9-digit code (3 city + 3 bank + 3 branch); magnetic ink at cheque bottom |
| **NEFT** | National Electronic Fund Transfer | Batch (not real-time) | RBI-maintained; one-to-one; add beneficiary first; all NEFT-enabled banks |
| **RTGS** | Real-Time Gross Settlement | Real-time (instant) | Fastest channel; no delay; high-value transfers; processed immediately |
| **CBS** | Core Banking Solutions | Real-time (centralised) | All branches interconnected; operate account from any branch; single platform |
| **ATM** | Automated Teller Machine | Instant | Cash dispensing via debit/credit card; magnetic strip; Any Time Banking |
| **Tele Banking** | — | 24-hour voice service | Customer care phone; block cards, account info, report loss anytime |
| **Internet Banking** | — | 24/7 online access | Bank website; username + password; fund transfer, FD info on laptop/PC |
| **Mobile Banking** | — | 24/7 on mobile app | Requires installed app; transactions, fund transfer, account info on phone |

#### 6.1.4 IT in Education

**Theory**

IT transforms education through seven areas. **Access to Study Material** — e-books, guides, previous question papers online as supplements. **Continuous Learning** — teachers send assignments online; students submit without physical classroom attendance. **Sharing of Knowledge** — online forums and social media for distance-independent collaboration. **Audio and Visual Learning Aids** — voice clips, YouTube, classroom videos for better understanding and practical demos. **Distance Learning** — online courses for all ages; overseas university courses from home. **Proper Record Keeping** — secure digital student records replacing manual files. **Video Conferencing** — virtual classes, seminars, meetings, training sessions from anywhere.

| Education IT Area | Description | Example |
|------------------|-------------|---------|
| Access to study material | E-books, guides, question papers online | SGOU SLM e-content |
| Continuous learning | Online assignments and submissions | Learning beyond classroom |
| Sharing of knowledge | Forums and social media collaboration | Distance-independent discussion |
| AV learning aids | Voice clips, YouTube, classroom videos | Practical demos of theory |
| Distance learning | Online courses for all ages | Overseas courses from home |
| Record keeping | Secure digital student records | Eliminates manual file loss |
| Video conferencing | Virtual classes and seminars | Quality education from anywhere |

**Important Points**

- E-books, guides, question papers accessible via Internet
- Online assignments enable learning anywhere, anytime
- AV aids: YouTube, voice clips, classroom videos
- Distance learning reaches populations unable to attend offline
- Digital records eliminate manual file loss
- Video conferencing delivers quality education remotely
- Online forums enable knowledge sharing across distances
- Overseas university courses accessible from home country

**For Exam**

IT in education enables access to electronic study materials (e-books, guides, previous question papers as supplements), continuous learning (teachers send assignments online; students submit without physical classroom attendance), knowledge sharing (online forums and social media for distance-independent collaboration), audio-visual learning aids (voice clips, YouTube, classroom videos for better understanding and practical demos), distance learning (online courses for all ages; overseas university courses from home), secure digital record keeping (eliminates manual file loss), and video conferencing (virtual classes, seminars, meetings, training sessions from anywhere).

#### 6.1.5 IT in the Medical Field

**Theory**

**Health Information Technology (HIT)** applies IT in healthcare using electronic devices to store, share, and analyse health information. Improves care quality, diagnostic accuracy; reduces costs and errors. **MPM (Medical Practice Management)** software manages administrative and clinical practice — appointments, insurance verification. **EHR/EMR** digitally documents patient medical records; eliminates manual charting errors; enables sharing when patients move hospitals. **RPM (Remote Patient Monitoring)** uses medical sensors (blood sugar, pressure, heartbeat) sending data to doctor's device for remote treatment of chronic patients. HIT defines management of information between doctors and patients.

| Medical IT System | Full Form | Function |
|------------------|-----------|----------|
| **HIT** | Health Information Technology | IT applied to healthcare overall |
| **MPM** | Medical Practice Management | Admin/clinical practice; appointments, insurance |
| **EHR** | Electronic Health Records | Digital patient records; shareable across hospitals |
| **EMR** | Electronic Medical Records | Documentation and storage of patient medical info |
| **RPM** | Remote Patient Monitoring | Sensors send vitals to doctor's device remotely |

**Important Points**

- HIT = IT applied to healthcare
- MPM automates appointments and insurance tasks
- EHR/EMR = digital patient records; shareable across hospitals
- RPM = sensors monitor vitals remotely
- HIT improves quality, accuracy; reduces costs and errors
- Telemedicine and online patient monitoring supported by IT
- EHR allows doctors to record on computer or mobile device
- RPM reduces costs and saves lives of chronic disease patients

**For Exam**

Health Information Technology applies IT in healthcare using electronic devices to store, share, and analyse health information by professionals. MPM software manages administrative and clinical practice — automates appointments and insurance verification. EHR/EMR digitally stores patient medical records on computer/mobile, eliminating manual charting errors and enabling sharing when patients move between hospitals. RPM uses medical sensors (blood sugar, pressure, heartbeat) to send data to doctor's mobile/laptop for remote treatment. HIT improves healthcare quality and diagnostic accuracy while reducing costs, errors, and enabling telemedicine for chronic patients.

#### 6.1.6 IT in Science

**Theory**

IT enables collection, storage, and processing of vast scientific data. Computations done in seconds (e.g. digits of Pi) that humans cannot complete in a lifetime. Detects particular data from millions of records. **Automated machines** (robotic arms) handle dangerous radioactive samples safely. Enables global collaboration — scientists share ideas worldwide. **Computer simulation** creates models and analyses results before physical laboratory experiments. Scientists can collaborate on projects with colleagues anywhere in the world without travel.

**Important Points**

- Fast computation and large-scale data processing
- Data detection from millions of records
- Robotic automation for dangerous sample handling
- Global scientific collaboration via networks
- Computer simulation before physical experiments
- IT stores and organises vast scientific information
- Robotic arms handle radioactive samples safely
- Simulation models tested before costly lab experiments

**For Exam**

IT in science enables fast computation (e.g. digits of Pi in seconds — work exceeding human lifetimes), detection of specific data from millions of records, automated machines (robotic arms handling dangerous radioactive samples safely), global collaboration among scientists sharing ideas worldwide, and computer simulation to create models and analyse results before costly physical laboratory experiments. IT stores and organises vast scientific information for different research purposes.

#### 6.1.7 Mobile Applications Development ⭐

**Theory**

Mobile application development creates software for mobile platforms. Three types: **Native Applications** — built for specific platform (e.g. Android) using platform tools; uses full device potential; examples: WhatsApp, Facebook. **HTML5 Applications** — web technologies (HTML5, JavaScript, CSS); write-once-run-anywhere; minimal changes per OS. **Hybrid Applications** — native container embedding HTML5 app; combines both approaches; examples: Twitter, Gmail, Instagram. Developers consider existing apps before creating new ones for greater impact.

**Important Points**

- Native = platform-specific; full device capability
- HTML5 = web-based; cross-platform compatibility
- Hybrid = native shell + HTML5 inside
- IT supports all three development approaches
- Native preferred for device integration (smart home apps)
- Hybrid uses native container with embedded web app
- HTML5 requires minimal changes for each operating system
- Native apps integrate with smart home devices for personalised experiences

**For Exam**

Mobile application development creates software for mobile platforms. Three types exist: Native applications are built for specific platforms (e.g. Android) using platform-specific tools, utilizing full device potential (WhatsApp, Facebook). HTML5 applications use web technologies (HTML5, JavaScript, CSS) with write-once-run-anywhere approach requiring minimal changes per OS. Hybrid applications combine native containers with embedded HTML5 apps (Twitter, Gmail, Instagram). IT advancement supports all three approaches for entertainment, business, and education apps.

| App Type | Platform | Technology | Advantages | Examples |
|----------|----------|-----------|------------|---------|
| **Native** | Specific (Android/iOS) | Platform SDK and languages | Full device potential; best performance | WhatsApp, Facebook |
| **HTML5** | Cross-platform | HTML5, JavaScript, CSS | Write-once-run-anywhere; minimal OS changes | Web-based mobile apps |
| **Hybrid** | Cross-platform | Native container + HTML5 | Best of both; unique native elements | Twitter, Gmail, Instagram |

### Unit Recap — Unit 1

- IT = processing, management, transfer, storage, protection, retrieval of information
- Business: communication, inventory, e-commerce, CRM, decision support, CCTV
- Banking: ECS, MICR, NEFT, RTGS, CBS, ATM, tele/internet/mobile banking
- Education: e-materials, distance learning, AV aids, video conferencing
- Medical: HIT, MPM, EHR/EMR, RPM
- Science: computation, simulation, robotic automation, global collaboration
- Mobile apps: Native, HTML5, Hybrid

### Unit 2: IT in Other Disciplines

#### 6.2.1 Bioinformatics

**Theory**

**Bioinformatics** combines biology and information technology. Term coined by **Paulien Hogeweg** in 1979. Uses computational tools to manage, analyse, and manipulate large biological datasets. Three components: (1) database creation for biological data storage; (2) algorithms and statistics for relationship analysis; (3) analysis of DNA, RNA, protein sequences, structures, gene expression. **Human Genome Project** (1990) advanced bioinformatics — ~3 billion base pairs across 60,000–100,000 genes. Applications: pharmaceuticals, preventive medicine, gene therapy, drug discovery, crop improvement.

| Bioinformatics Application | Description |
|---------------------------|-------------|
| **Pharmaceuticals** | Drug discovery; personalized medicine for infectious diseases |
| **Preventive medicine** | Combined with epidemiology; understand disease patterns |
| **Gene therapy** | Incorporate genetic materials into diseased/unhealthy cells |
| **Drug discovery** | Computational biology validates cost-effective drugs |
| **Crop improvement** | Drought-resistant and insect-resistant crop development |

**Important Points**

- Bioinformatics = IT + biology
- Three components: databases, algorithms/statistics, data analysis
- Coined by Paulien Hogeweg (1979)
- Human Genome Project drove genome-stage development
- Applications: pharma, gene therapy, drug discovery, crop improvement
- Computers essential for processing billions of base pairs
- Gene therapy incorporates genetic materials into diseased cells
- Crop improvement: drought-resistant and insect-resistant varieties

| Bioinformatics Component | Description |
|---------------------------|-------------|
| **Database creation** | Storage and management of large biological data sets |
| **Algorithms & statistics** | Determine relationships among members of large data sets |
| **Data analysis tools** | Analyse DNA, RNA, protein sequences, structures, gene expression |

**For Exam**

Bioinformatics is the combination of biology and information technology, coined by Paulien Hogeweg in 1979. It encompasses database creation for biological data storage, algorithm/statistics development for relationship analysis, and analysis of biological data (DNA, RNA, protein sequences, structures, gene expression profiles). The Human Genome Project (1990) advanced bioinformatics — 23 chromosomes, 60,000–100,000 genes, ~3 billion base pairs. Applications include pharmaceuticals (personalized medicine), preventive medicine (epidemiology), gene therapy (incorporating genetic materials into diseased cells), drug discovery (computational biology), and crop improvement (drought/insect-resistant crops).

#### 6.2.2 IT in Medicine

**Theory**

IT in medicine includes: **Hospital Information System (HIS)** — manages registration, billing, medical records, pharmacy, payroll across hospital departments. **Data Analysis** — statistical calculations on large medical research data in seconds. **Laboratory Computing** — accurate blood chemistry, microbiology results linked to patient IDs. **CADM (Computer-Assisted Decision Making)** — interactive system assisting doctors with clinical decisions using computer memory and processing. **Critical Care** — computerised vital sign monitoring in ICU. **Computer-Assisted Therapy** — dosage planning for toxic drugs. **Medical Imaging** — CT, MRI, ultrasound, 3D anatomy via dedicated hardware/software. **Computer-Aided Diagnostics (CAD)** — assists interpretation of X-ray, MRI images; detects breast cancer, lung tumors.

| Medicine IT Application | Description |
|------------------------|-------------|
| **HIS** | Hospital registration, billing, records, pharmacy, payroll |
| **Data Analysis** | Statistical calculations on large medical research datasets |
| **Laboratory Computing** | Blood chemistry, microbiology results linked to patient IDs |
| **CADM** | Interactive system assisting doctors with clinical decisions |
| **Critical Care (ICU)** | Computerised vital sign, medication, lab value monitoring |
| **Computer-Assisted Therapy** | Dosage planning for powerful/toxic drugs |
| **Medical Imaging** | CT, MRI, ultrasound, 3D anatomy generation |
| **CAD / CADe** | Assists medical image interpretation; detects cancer/tumors |

**Important Points**

- HIS covers registration, billing, records, pharmacy, payroll
- CADM assists clinical decision-making tasks
- Medical imaging: CT, MRI, ultrasound, gamma cameras
- CAD/CADe highlights suspicious areas in medical images
- Laboratory computing delivers fast, accurate results
- ICU data management: vitals, medications, lab values
- CAD detects breast cancer on mammography, lung tumors on CT
- Closed-loop systems control drug infusion based on patient vitals

**For Exam**

IT in medicine includes Hospital Information Systems (registration, admission/discharge, billing, medical records, pharmacy, payroll), computer-assisted data analysis (statistical calculations on large research data in seconds), laboratory computing (blood chemistry, microbiology linked to patient IDs), CADM (interactive system assisting doctors with clinical decisions using computer memory/reliability), computerised ICU vital sign monitoring, computer-assisted therapy (dosage planning for toxic drugs), medical imaging (CT, MRI, ultrasound, 3D anatomy), and computer-aided diagnostics/CAD (assists X-ray/MRI interpretation; detects breast cancer on mammography, lung tumors on CT scans).

#### 6.2.3 Computational Economics and Finance

**Theory**

**Computational Economics** is interdisciplinary (computer science, economics, management science) involving computational modelling of economic systems. **Computational Finance** combines mathematical science, economic theory, statistics, and computer simulation for investment planning and risk management. **Economic Forecasting** uses computer simulations to predict market changes. **Online Trading/E-commerce** enables instant digital transactions. **Stock Markets** — online trading apps, stock prediction robots, faster transactions, real-time monitoring, enhanced security, **Blockchain** for secure trading (SEBI exploring adoption). Blockchain eliminates third-party authorities using smart contracts.

**Important Points**

- Computational Economics = computational modelling of economic systems
- Computational Finance = simulation for investment and risk management
- Forecasting models predict market changes rapidly
- Online trading apps eliminate brokers and paperwork
- Blockchain enables secure, transparent stock transactions
- Real-time monitoring gives accurate prices instantly
- Automated robots analyse thousands of data points for stock prediction
- SEBI exploring blockchain for Indian stock market infrastructure

**For Exam**

Computational economics uses computer science, economics, and management science to computationally model economic systems and develop strategies. Computational finance combines mathematical science, economic theory, statistics, and simulation for investment planning and risk management. Economic forecasting uses computer models to predict market changes rapidly. IT revolutionised stock markets through online trading apps (no broker/paperwork), automated stock prediction robots, faster secure transactions, real-time price monitoring, enhanced security, and blockchain technology (SEBI exploring adoption for transparent, smart-contract-based trading).

| Stock Market IT Application | Description |
|----------------------------|-------------|
| **Online trading apps** | Direct trading without broker; hassle-free, lower costs |
| **Stock prediction robots** | Analyse thousands of data points; execute at minimal prices |
| **Faster transactions** | Eliminates manual records, audits, verification delays |
| **Real-time monitoring** | Accurate trusted prices; investors react quickly to market changes |
| **Enhanced security** | Complete transaction records; trust and transparency |
| **Blockchain** | Secure trading via smart contracts; SEBI exploring adoption in India |

#### 6.2.4 Cognitive Science and AI Applications 🔥

**Theory**

**Cognitive Science and AI** integrates AI with human cognition study — language, reasoning, learning, vision, human-technology interaction, AI ethics. **Speech-to-text** converts spoken audio to text; **text-to-speech** converts text to speech (Google Assistant, Voice Aloud Reader). **Personaliser** (Microsoft Azure) uses reinforcement learning for personalised content recommendations. AI lifestyle applications: autonomous vehicles (Tesla, Toyota, Volvo), spam filters (Gmail 99.9%), facial recognition, recommendation systems (YouTube, e-commerce), GPS navigation (Uber route optimisation using CNN and GNN).

| Cognitive AI Application | Description | Real-World Example |
|-------------------------|-------------|-------------------|
| **Speech-to-text** | Converts spoken audio into text; real-time streaming | Conversation transcription APIs |
| **Text-to-speech** | Converts written text into spoken audio | Google Assistant, Voice Aloud Reader |
| **Personaliser** | Reinforcement learning for content recommendations | Microsoft Azure Personaliser Preview |
| **Autonomous vehicles** | Machine learning for driving and object detection | Toyota, Audi, Volvo, Tesla |
| **Spam filters** | AI filters unwanted email automatically | Gmail ~99.9% filtration capacity |
| **Facial recognition** | Detects and identifies faces for secure access | Phone unlock, high-security areas |
| **Recommendation systems** | Analyses user behaviour for customised content | YouTube, e-commerce platforms |
| **GPS navigation** | CNN + GNN for route detection and optimisation | Uber, logistics companies |

**Important Points**

- Cognitive science AI = AI + human cognition study
- Speech-to-text and text-to-speech are key applications
- Personaliser delivers customised user experiences
- Autonomous vehicles use machine learning
- Spam filters and facial recognition use AI daily
- Recommendation systems analyse user behaviour
- Personaliser uses reinforcement learning (Microsoft Azure)
- GPS combines Convolutional Neural Network and Graph Neural Network

**For Exam**

Cognitive science integrates artificial intelligence with the study of human cognition covering language, reasoning, learning, vision, and human-technology interaction. Key applications include speech-to-text (converts spoken audio; real-time streaming transcription), text-to-speech (Google Assistant, Voice Aloud Reader), and Personaliser (Microsoft Azure reinforcement learning for customised content). AI lifestyle applications include autonomous vehicles (Toyota, Audi, Volvo, Tesla — machine learning for driving and object detection), spam filters (Gmail 99.9% filtration), facial recognition (phones, high-security areas), recommendation systems (YouTube, e-commerce analyse browsing history), and GPS navigation (Uber uses CNN and GNN for route optimisation).

#### 6.2.5 Quantum Computing

**Theory**

**Quantum computing** harnesses quantum mechanics to solve problems too complex for classical computers. Uses **qubits** — quantum bits existing in multiple states simultaneously (unlike classical bits 0 or 1). Emerged in 1980s; companies: IBM, Google, Microsoft, Intel, Alibaba, Nokia. **Silq** is a high-level programming language for quantum computing developed at ETH Zürich. AI, machine learning, and big data search combine with quantum computing. Applications: complex problem solving, secure data encryption, detecting intruders via light signals. QIST (Quantum Information Science and Technology) combines quantum mechanics with information technology.

| Concept | Classical Computing | Quantum Computing |
|---------|--------------------|--------------------|
| **Basic unit** | Bit (0 or 1 only) | Qubit (multiple states simultaneously) |
| **Programming language** | C, Python, Java, etc. | Silq (ETH Zürich) |
| **Emergence** | 1940s onwards | 1980s |
| **Key companies** | Intel, AMD | IBM, Google, Microsoft, D-Wave |
| **Applications** | General computing | Complex problems, encryption, AI/ML integration |

**Important Points**

- Qubits exist in multiple states simultaneously
- Classical bits = 0 or 1; qubits = multidimensional quantum state
- Silq = programming language for quantum computing
- Field emerged in 1980s
- Used with AI, ML, and big data search
- Companies: IBM, Google, Microsoft, Intel
- QIST = Quantum Information Science and Technology
- Quantum algorithms tackle problems faster than classical counterparts

**For Exam**

Quantum computing uses quantum mechanics and qubits (quantum bits that exist in multiple states simultaneously) to solve complex problems beyond classical computers. Unlike classical bits (0 or 1 only), qubits engage 0 and 1 multidimensionally. The field emerged in the 1980s when quantum algorithms were found more efficient than classical ones for certain problems. Silq is a high-level programming language for quantum computing developed at ETH Zürich with a strong static type system. It combines with AI, machine learning, big data search, and secure data encryption. Companies investing in quantum computing include IBM, Google, Microsoft, Intel, and Alibaba.

#### 6.2.6 Nanotechnology

**Theory**

**Nanotechnology** is science/engineering at the **nanoscale** (1–100 nanometers; 1 nm = 10⁻⁹ meter). Involves seeing and controlling individual atoms and molecules. Tools: STM (Scanning Tunneling Microscope), AFM (Atomic Force Microscope) invented in early 1980s. IT applications: **data exploration and visualization** (real-time interactive environments), **computational geometry** (specialized algorithms for nanoscale geometries), **software usage** (open-source, object-oriented codes for simulation and analysis on multiple platforms). Medieval stained glass used alternate-sized gold/silver nanoparticles for colour.

**Important Points**

- Nanoscale = 1 to 100 nanometers
- STM and AFM enable nanoscale observation
- IT provides data visualization and exploration tools
- Computational geometry algorithms for nanoscale structures
- Open-source modular software essential for nanotech simulation
- Enhanced properties: strength, lightness, chemical reactivity
- Nanoscale materials used for centuries in stained glass windows
- Real-time data interactivity hides complexity from the user

**For Exam**

Nanotechnology operates at 1–100 nanometers (1 nm = 10⁻⁹ meter), studying and manipulating individual atoms and molecules. Tools like STM (Scanning Tunneling Microscope) and AFM (Atomic Force Microscope) invented in the early 1980s enabled the nanotechnology age. Medieval stained glass used gold/silver nanoparticles for colour centuries ago. IT contributes through data exploration and visualization (real-time interactive environments hiding data complexity), computational geometry algorithms for nanoscale structures, and open-source object-oriented modular software for simulation and analysis across platforms.

### Unit Recap — Unit 2

- Bioinformatics = IT + biology; databases, algorithms, analysis
- Medicine: HIS, CADM, medical imaging, computer-aided diagnostics
- Computational economics/finance: modelling, forecasting, online trading
- Cognitive science AI: speech-to-text, text-to-speech, personaliser
- Quantum computing: qubits, Silq programming language
- Nanotechnology: nanoscale; IT for visualization and computational geometry

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

### Unit 4: Latest Trends in Computer Science

#### 6.4.1 Virtual Reality (VR) 🔥

**Theory**

**Virtual Reality (VR)** creates a simulated virtual environment — an alternate world of reality using IT. User feels immersed in imaginary surroundings via VR headsets, gloves, and sensory equipment tracking head/eye movements. Setup: VR headset (A), battery pack (B), controller box (C), laptop (D), USB/HDMI cables (E, F). Three types: **Fully-Immersive** (most realistic; gaming/entertainment; HTC Vive, PlayStation VR), **Semi-Immersive** (partial virtual; education/training with projectors), **Non-Immersive** (common video games). Benefits: immersive learning, interactive atmosphere, realistic exploration, skill enhancement. Real Reality = actual world; Virtual Reality = imaginary world created with IT.

| VR Type | Description | Use Case | Examples |
|---------|-------------|----------|---------|
| **Fully-Immersive** | Most realistic; high-resolution; wide field of view | Gaming, entertainment | HTC Vive, PlayStation VR |
| **Semi-Immersive** | Partially virtual; computer graphics + projectors | Education, training | Large projector systems |
| **Non-Immersive** | Least immersive; standard screen-based | Everyday video games | Average PC/console games |

**Important Points**

- VR = simulated virtual environment; user feels immersed
- Equipment: VR headset, gloves, controller box, laptop
- Three types: Fully-Immersive, Semi-Immersive, Non-Immersive
- Examples: HTC Vive, PlayStation VR
- Applications: 3D movies, gaming, education, science
- Tracks head and eye movements for immersion
- Two lenses between screen adjust to eye movement
- Uses video, audio, and haptic (touch) simulations

**For Exam**

Virtual Reality creates a simulated virtual environment using computers and sensory equipment (VR headsets, gloves, controller box, laptop). The user experiences an alternate world with vision, hearing, and touch senses — e.g. experiencing Mars, swimming with sharks at home. Three types: Fully-Immersive (most realistic; gaming/entertainment; HTC Vive, PlayStation VR), Semi-Immersive (partial virtual; education/training with projectors), and Non-Immersive (standard video games). Setup: VR headset blocks real world; HDMI connects laptop; lenses adjust to eye movement. Benefits: immersive learning, interactive atmosphere, realistic exploration, skill enhancement, comfortable education.

#### 6.4.2 Augmented Reality (AR) 🔥

**Theory**

**Augmented Reality (AR)** enhances real-world objects with digital content (images, sounds, text) creating interactive experiences. Unlike VR (fully virtual), AR exists in the real world — like using a magnifying glass or smartphone zoom to enhance viewing. Setup: camera captures real world → video merger combines with virtual objects from graphics system → augmented stream to user. Devices: **HUD** (Head Up Display — complex info in small area), Smart Glasses, Holographic Display, Smartphones. Four types: **Marker Based** (QR codes), **Superimposed/Markerless** (virtual objects on physical world), **Location Based** (GPS/compass; Google Maps), **Projection Based** (interactive hologram).

| AR Type | Mechanism | Example |
|---------|-----------|---------|
| **Marker Based** | Visual markers (QR codes) connect digital to real world | QR code scanning |
| **Superimposed / Markerless** | Virtual objects superimposed on physical world | Move virtual objects in real space |
| **Location Based** | GPS, compass provide location-specific data | Google Maps navigation |
| **Projection Based** | Light projected on surfaces; senses human interaction | Interactive hologram |

**Important Points**

- AR = real world enhanced with digital objects
- VR = fully virtual; AR = real world augmented
- Devices: HUD, Smart Glasses, Holographic Display, Smartphones
- Four types: Marker Based, Superimposed, Location Based, Projection Based
- Camera + graphics system + video merger = AR pipeline
- Benefits: education, healthcare, gaming, accuracy, remote sharing
- HUD shows complex info while interacting with real environment
- Holographic display needs no wearable device

**For Exam**

Augmented Reality generates interactive experiences by enhancing real-world objects with digital content (images, sounds, text). Unlike VR which creates fully virtual environments, AR superimposes digital elements on the real world — like a magnifying glass enhancing a document. Setup: camera captures real world → video merger combines with virtual objects from graphics system → augmented stream to user. Devices: HUD (complex info in small area), Smart Glasses, Holographic Display (3D space, no wearable), Smartphones. Four types: Marker Based (QR codes connect digital to real), Superimposed/Markerless (virtual objects on physical world), Location Based (GPS/compass; Google Maps), Projection Based (interactive hologram with light projection).

| Feature | Virtual Reality (VR) | Augmented Reality (AR) |
|---------|---------------------|------------------------|
| **Environment** | Fully simulated/virtual world | Real world enhanced with digital objects |
| **User experience** | Immersed in imaginary surroundings | Sees real world + overlaid digital content |
| **Equipment** | VR headset, gloves, controller box, laptop | HUD, Smart Glasses, Smartphone, Holographic display |
| **Setup** | Headset blocks real world; HDMI to laptop | Camera → video merger → augmented stream |
| **Types** | Fully-Immersive, Semi-Immersive, Non-Immersive | Marker Based, Superimposed, Location Based, Projection Based |
| **Examples** | HTC Vive, PlayStation VR, 3D gaming | QR codes, Google Maps, interactive hologram |
| **Applications** | Gaming, 3D movies, education, science | Education, healthcare, gaming, navigation |
| **Key difference** | Creates alternate reality | Augments existing reality |

#### 6.4.3 Artificial Intelligence (AI) and Automation 🔥

**Theory**

**AI** was coined by **John McCarthy in 1956** — "Science and Engineering of making intelligent machines." Machines work and behave like humans using data and algorithms. **Automation** = production/delivery of goods/services with minimal human intervention. AI works by: perceive environment (data) → detect patterns → learn from patterns → repeat until confident predictions (Fig 6.4.4). Three types: **Narrow/Weak AI** (specific tasks — Alexa, face verification, Google Maps), **General/Strong AI** (any intellectual task like humans; not yet achieved), **Super AI** (exceeds human ability; hypothetical/science fiction). Applications: healthcare (Fitbit), automobiles (self-driving), surveillance, social media, entertainment, education.

| AI Application Area | Example | How AI Is Used |
|--------------------|---------|---------------|
| **Healthcare** | Fitbit, iWatch | Early disease detection; doctor decision support |
| **Automobiles** | Tesla, Toyota, Volvo | Self-driving; object detection; route optimisation |
| **Surveillance** | Face recognition tools | Observation and security in public/industrial areas |
| **Social Media** | Facebook, Twitter, Google | Personalised feeds; hate speech detection |
| **Entertainment** | YouTube, Netflix | Recommendations based on viewing history |
| **Education** | AI monitoring systems | Track academic, psychological, physical student wellbeing |

**Important Points**

- AI coined by John McCarthy (1956)
- Three types: Narrow (Weak), General (Strong), Super AI
- Working: perceive → detect patterns → learn → predict
- Narrow AI examples: Alexa, Google Maps, face verification
- Automation = minimal human intervention in production
- Applications: healthcare, automobiles, surveillance, social media, education
- Google AI eye doctor detects diabetic retinopathy from retina scans
- Twitter AI identifies hate speech and terrorist language

**For Exam**

Artificial Intelligence, coined by John McCarthy in 1956 ("Science and Engineering of making intelligent machines"), makes machines work like humans by processing data through algorithms adjusted by past experiences. Three types: Narrow AI (specific tasks — Alexa operates in limited predefined range, no self-awareness; Google Maps, face verification), General AI (any intellectual task like humans; high computation but cannot yet think/reason like humans), and Super AI (exceeds human ability; hypothetical as in science fiction). AI workflow: perceive environment (data) → detect patterns → learn from patterns → repeat until confident predictions. Automation delivers goods/services with minimal human intervention. Applications: healthcare (Fitbit early disease detection), self-driving cars, surveillance (face recognition), social media (Facebook feeds, Twitter hate speech detection), entertainment (streaming recommendations), education (student wellbeing monitoring).

| AI Type | Also Called | Capability | Status | Examples |
|---------|------------|------------|--------|---------|
| **Artificial Narrow Intelligence** | Weak AI | Specific tasks only; predefined range | Currently exists | Alexa, Google Maps, face verification, Siri |
| **Artificial General Intelligence** | Strong AI | Any intellectual task like a human | Not yet achieved | Hypothetical human-level reasoning machines |
| **Artificial Super Intelligence** | Super AI | Exceeds human cognitive ability | Hypothetical/sci-fi | Machines surpassing humans in all tasks |

#### 6.4.4 Smart Technology

**Theory**

**Smart Technology** — "SMART" = **Self-Monitoring, Analysis, and Reporting Technology** using AI and Machine Learning for intellectual awareness. Three types: **IoT Devices** — sensors, gateway, software, servers, UI bringing physical objects to life (smart cities, smart homes). **Smart Connected Devices** — controlled via remote/smartphone over Internet/Bluetooth/WiFi; customized but less adaptive (smart cameras, smart bulbs). **Smart Devices** — limited automation, no Internet required, programmable (smart coffee makers). Amazon Echo enables voice control of smart fan. Benefits: accessibility, sustainability, security, efficiency, saves time and money.

| Smart Technology Type | Connectivity | Adaptability | Examples |
|----------------------|-------------|-------------|---------|
| **IoT Devices** | Internet; sensors + gateway + server | Most adaptive to user behaviour | Smart cities, smart homes |
| **Smart Connected Devices** | Internet / Bluetooth / WiFi | Customized but less adaptive | Smart cameras, smart bulbs |
| **Smart Devices** | No Internet required | Limited automation; programmable | Smart coffee makers, Amazon Echo |

**Important Points**

- SMART = Self-Monitoring, Analysis, and Reporting Technology
- Uses AI and Machine Learning
- Three types: IoT devices, Smart Connected Devices, Smart Devices
- IoT most adaptive; Smart Connected via remote/app
- Smart Devices need no Internet
- Examples: Amazon Echo (voice control), smart TV, smartwatch
- Smart Connected uses Internet, Bluetooth, or WiFi
- IoT devices most capable of adapting to user behaviour

**For Exam**

Smart Technology (SMART = Self-Monitoring, Analysis, and Reporting Technology) uses AI and Machine Learning to give objects intellectual awareness so they perform smartly. Three types: IoT devices (network of sensors, gateway, software, servers, UI — most adaptive; smart cities/homes), Smart Connected Devices (remote/smartphone controlled via Internet/Bluetooth/WiFi — smart cameras/bulbs; customized but less adaptive), and Smart Devices (limited automation, no Internet, programmable — smart coffee makers). Amazon Echo enables voice control of appliances. Benefits: accessibility, sustainability, security, efficiency, saves time and money.

#### 6.4.5 Internet of Things (IoT) 🔥

**Theory**

**IoT** = system of interconnected computing devices, machines, animals, or people with **UIDs (Unique Identifiers)** transferring data over a network without human-to-human or human-to-computer interaction. A "thing" can be a heartbeat monitor implant, biochip animal, automobile tyre sensor, etc. **Four components:** Sensors, Gateway, Server, Mobile/Laptop. Example: soil moisture sensor detects dry soil → gateway sends data → server triggers sprinkler → notification sent to phone. IoT enables man-to-machine and machine-to-machine interactions simultaneously. **Cloud computing** (Amazon Web Services — AWS) delivers on-demand servers, storage, and databases over the Internet — a related trend in modern IT alongside IoT, VR, AR, and AI.

**IoT Workflow (5 Steps):**

1. **Collect Data** — Sensors/IoT devices gather environmental data (temperature, moisture, heartbeat, pressure)
2. **Transport Data** — Gateway receives sensor data and sends via WiFi, Bluetooth, mobile, or satellite network
3. **Process Data** — Server runs data processing software on the acquired information
4. **Trigger Action** — Server triggers automated response (e.g. turn on sprinkler when soil is dry)
5. **Notify User** — Processed information delivered to mobile/laptop via alarms, texts, or email notifications

| IoT Component | Role | Examples |
|--------------|------|---------|
| **Sensors** | Collect environmental/physical data | Temperature, moisture, heartbeat, tyre pressure sensors |
| **Gateway** | Transport data to server | WiFi, Bluetooth, mobile network, satellite |
| **Server** | Process data; trigger automated actions | Sprinkler activation when soil moisture drops |
| **Mobile/Laptop** | Display results; notify user | Alarms, SMS, email notifications on smartphone |

| IoT Application Area | Use Case |
|---------------------|----------|
| **Smart Homes** | Control lights, fan, AC, TV, washing machine via smartphone |
| **Wearables** | Smartwatch tracks heartbeat, oxygen, pressure; public safety routing |
| **Healthcare** | Remote patient monitoring; pharmaceutical inventory management |
| **Agriculture** | Soil moisture sensors trigger automated irrigation |
| **Smart Cities** | Smart streetlights; occupancy-based AC temperature adjustment |
| **Automobile** | Tyre pressure sensors alert driver via network |

**Important Points**

- IoT = interconnected things with UIDs transferring data automatically
- Four components: Sensors, Gateway, Server, Mobile/Laptop
- Gateway options: WiFi, Bluetooth, mobile/satellite networks
- No human-to-human interaction required
- Applications: smart homes, wearables, healthcare, agriculture, smart cities
- Benefits: remote access, automation, time/money savings
- UID = unique identification number for each IoT device
- Choose gateway based on power consumption, range, and bandwidth

**For Exam**

Internet of Things (IoT) is a system of interconnected devices with unique identifiers (UIDs) that collect and transfer data over networks without human-to-human or human-to-computer interaction. Four components: Sensors (collect environmental data — temperature, heartbeat, moisture), Gateway (transports via WiFi/Bluetooth/mobile/satellite; choose based on power, range, bandwidth), Server (processes data and triggers automated actions), and Mobile/Laptop (delivers results via alarms/notifications). Workflow: (1) Collect → (2) Transport → (3) Process → (4) Trigger Action → (5) Notify User. Example: soil moisture sensor → gateway → server turns on sprinkler → report to phone. Applications: smart homes, wearables, healthcare, agriculture, smart cities. IoT enables automation, remote access, and improved service quality. **Cloud computing** (e.g. Amazon Web Services — AWS) delivers on-demand IT resources (servers, storage, databases) over the Internet without physical hardware — another key trend alongside VR, AR, AI, and IoT.

### Unit Recap — Unit 4

- VR = fully virtual simulated environment; three immersion levels
- AR = real world enhanced with digital objects; four types
- AI (McCarthy 1956): Narrow, General, Super AI; perceive-learn-predict
- Smart Technology: IoT devices, Smart Connected, Smart Devices
- IoT: Sensors → Gateway → Server → Mobile; UIDs identify things
- Cloud computing (AWS) = on-demand IT resources over Internet

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

## Block 1 Revision Checklist

- [ ] 🔥 Four functions of a computer: Input, Processing, Output, Storage
- [ ] Hardware, Software, Firmware (BIOS/POST), Liveware
- [ ] Block diagram: Input unit → CPU (CU, ALU, Memory) → Output unit
- [ ] 🔥 Von-Neumann architecture and stored program concept (1945)
- [ ] Processor, Motherboard, Memory (RAM/ROM types), Registers, SMPS
- [ ] Binary (base-2), Decimal (base-10), Octal (base-8), Hex (base-16)
- [ ] Bit, Nibble (4 bits), Byte (8 bits), MSB, LSD
- [ ] 🔥 BCD, Gray code, Excess-3, ASCII (A=65, a=97)
- [ ] Input devices: Keyboard, Mouse, Touchpad, Scanner, Barcode reader
- [ ] Output devices: Monitor (soft), Printer/Plotter (hard), Speakers (audio)
- [ ] Impact vs Non-impact printers; Laser vs Dot matrix
- [ ] Evolution: Abacus → Pascaline → Babbage → ABC → Transistors → IC → Microcomputer
- [ ] 🔥 Analog vs Digital vs Hybrid computers
- [ ] Types by size: Laptop, PC, Workstation, Mainframe, Supercomputer, Handheld, Wearable

## Block 2 Revision Checklist

- [ ] Memory structure: cells (1 bit), addresses, memory words
- [ ] Units: KB, MB, GB, TB, PB (× 1024 each)
- [ ] Read/Write operations; access time
- [ ] Primary memory: RAM (volatile), ROM (non-volatile)
- [ ] 🔥 SRAM vs DRAM comparison table
- [ ] 🔥 Cache: L1/L2/L3, hit/miss/penalty, hit ratio formula
- [ ] 🔥 Memory hierarchy: Registers → Cache → Main → Secondary → Offline
- [ ] Instruction set and ISA; opcode + address fields
- [ ] 🔥 Instruction cycle: Fetch → Decode → Operand Fetch → Execute
- [ ] 🔥 RISC vs CISC comparison (simple/fast vs complex/compact)
- [ ] 🔥 CPU registers: MAR, MDR, PC, IR, Accumulator, GPR, Flags
- [ ] 🔥 Virtual memory: virtual vs physical/logical addresses
- [ ] Secondary storage characteristics: non-volatile, large, cheap
- [ ] Magnetic tape vs disk; HDD specs (rpm, capacity)
- [ ] Optical media: CD, DVD, Blu-ray capacities
- [ ] USB, pen drive, external HDD, memory stick, SSD
- [ ] Number conversions: decimal↔binary, binary↔hex, decimal↔octal
- [ ] Digital codes comparison: BCD, Gray, Excess-3, ASCII
- [ ] Memory hierarchy access times (registers ns → tape seconds)
- [ ] Instruction cycle phases with register roles (PC, IR, MAR, MDR)
- [ ] Secondary storage capacity table (CD 700MB → Blu-ray 50GB → SSD TB)

## Block 3 Revision Checklist

- [ ] Define software; distinguish instruction, program, hardware, software
- [ ] 🔥 Classify software: System vs Application with comparison table
- [ ] Distinguish static vs dynamic websites with examples
- [ ] Explain website access flow (browser → Internet → web server → display)
- [ ] List OS functions with descriptions (process, memory, file, device management)
- [ ] Explain device drivers and language processors as system software
- [ ] Describe files (name, extension, path, metadata) and folders (directories, subfolders)
- [ ] 🔥 List boot process steps in order (power on through ready state)
- [ ] Explain BIOS role and boot device priority
- [ ] 🔥 Define booting; compare warm (soft reboot) vs cold (hard booting)
- [ ] 🔥 Explain POST and what hardware it checks
- [ ] 🔥 Describe three software layers: Presentation, Application, Data
- [ ] Compare one-tier, two-tier, three-tier architecture
- [ ] Define OS; explain DOS (command-based, single-user, single-task)
- [ ] Explain client-server model with restaurant analogy
- [ ] 🔥 List and describe 7 OS types: Batch, Time-sharing, Multiprocessing, Real-time, Distributed, Network, Mobile
- [ ] Compare Linux vs Windows (open source, cost, case sensitivity, security)
- [ ] Describe Android (Linux kernel) and iOS (Apple)
- [ ] Define GUI and its advantages over command interface
- [ ] Classify programming languages: High level vs Low level (Assembly, Machine)
- [ ] 🔥 Compare Compiler vs Interpreter vs Assembler
- [ ] Define database and DBMS with advantages
- [ ] List utility software examples (antivirus, backup, disk tools)
- [ ] Describe application software types: word processor, spreadsheet, presentation, LaTeX
- [ ] 🔥 Define computer virus, entry methods, types, and protection measures

## Block 4 Revision Checklist

- [ ] Define computer network; explain communication model (sender, medium, receiver)
- [ ] Distinguish guided vs unguided transmission media
- [ ] List network advantages: file sharing, hardware sharing, application sharing, messaging
- [ ] Explain basic network working with switch and shared printer
- [ ] 🔥 Compare LAN, MAN, WAN with examples
- [ ] 🔥 Compare Hub (broadcast) vs Switch (intelligent forward) vs Router (connects networks)
- [ ] Explain Repeater (signal boost) and Bridge (segment division)
- [ ] 🔥 Draw/describe ASCII for all six topologies (Bus, Ring, Star, Mesh, Tree, Hybrid)
- [ ] Explain ring topology token system
- [ ] Compare Peer-to-Peer vs Client/Server NOS
- [ ] Trace Internet history: ARPA, ARPANET, TCP, NSFNET, HTTP, Mosaic
- [ ] Define Internet, WWW, web page, website, URL, browser, search engine
- [ ] 🔥 Explain URL parts: protocol, domain, extension, page
- [ ] Describe search engine working with web crawler/spider
- [ ] List Internet search tips: keywords, quotes, Boolean, Ctrl+F
- [ ] Define ISP and its services (access, domain, hosting, Usenet)
- [ ] Compare connection types with speed/cost table: Dial-up, Cable, WLL, Broadband, Leased Line
- [ ] Explain Wi-Fi vs WiMAX; DSL symmetric vs asymmetric; fibre vs satellite
- [ ] Describe email components: UA, MTA, Mailbox, Spool file
- [ ] 🔥 Compare email protocols: SMTP (send), POP3 (local receive), IMAP (server sync)
- [ ] Explain DSL splitter and symmetric vs asymmetric DSL
- [ ] Describe dial-up circuit switching and modem analog conversion
- [ ] Compare SMTP vs POP3 vs IMAP (send vs local receive vs server sync)
- [ ] Explain email address format username@domainname
- [ ] List email system services: Composition, Transfer, Reporting, Displaying, Disposition
- [ ] Describe WLL components: PSTN, Switch Function, WANU, WASU
- [ ] Compare fibre optics structure: jacket, cladding, core
- [ ] Explain CC vs BCC; email filtering, attach, and forward
- [ ] List web application benefits and characteristics (mobile, social, analytics)
- [ ] Name nine types of web pages

## Block 5 Revision Checklist

- [ ] Define HTML, Hypertext, Markup Language; list versions to HTML5
- [ ] 🔥 Draw HTML structure: DOCTYPE, html, head, title, body
- [ ] Compare Transitional, Strict, Frameset document types
- [ ] State five HTML coding rules and element syntax with attributes
- [ ] List head elements: title, style, base, link, meta — with purpose
- [ ] Differentiate title tag vs h1; explain div and center tags
- [ ] 🔥 Create ul, ol, dl lists with li, dt, dd tags
- [ ] Build table with tr, td, th; explain colspan/rowspan
- [ ] 🔥 Explain frameset/frame with cols/rows attributes
- [ ] Use img (src, alt), hex/RGB colours, marquee, audio/video tags
- [ ] 🔥 Write anchor links: internal (#id) and external (href URL)
- [ ] List 11 website creation steps including Bootstrap
- [ ] Know HTML global attributes: id, class, style, title, lang
- [ ] Reference HTML Quick Reference table for tag attributes

## Block 6 Revision Checklist

- [ ] Define IT and list associated terms (hardware, software, database, server, network)
- [ ] Explain IT in business: communication, inventory, e-commerce, CRM, decision support, CCTV
- [ ] Describe banking IT table: ECS, MICR, NEFT, RTGS, CBS, ATM, tele/internet/mobile banking
- [ ] List IT in education: study materials, continuous learning, distance learning, video conferencing
- [ ] Explain HIT, MPM, EHR/EMR, RPM in medical field
- [ ] Differentiate Native, HTML5, and Hybrid mobile applications
- [ ] Define bioinformatics (3 components) and IT in medicine (HIS, CADM, CAD)
- [ ] Explain computational economics, finance, forecasting, stock markets, blockchain
- [ ] Describe cognitive science AI, quantum computing (qubits, Silq), nanotechnology
- [ ] List six security measures and four computer security threats
- [ ] 🔥 Explain CIA triad: Confidentiality, Integrity, Availability
- [ ] 🔥 Define malware types and eight computer virus types (table)
- [ ] 🔥 Describe antivirus functions; compare VR and AR types
- [ ] 🔥 Explain AI types (Narrow, General, Super) and how AI works
- [ ] 🔥 Define Smart Technology types and IoT components/workflow/applications
- [ ] Explain cloud computing (AWS) as on-demand IT resource delivery
- [ ] Use Block 6 Quick Reference table for last-minute revision

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

## About the Author

**Abdul Vahab A A**  
Website: https://abdulvahabaa.in

Thank you for using these notes. I hope this Introduction to Information Technology file supports your semester learning, revision, and exam confidence.

**All the best for your exams and future in IT.** Keep learning consistently and trust your effort.

**Duaon mein Yaad Rakhna.**

---

### If These Notes Helped You — Say Thanks on WhatsApp

If this file helped you study or pass your exams, a small thank-you message means a lot. You can copy and send this:

```
Hi Abdul, your BCA Introduction to Information Technology study notes were really helpful. Thank you so much! Wishing you success too.
```

Share your feedback or suggestions anytime — it helps improve notes for other students too.

---

*Study notes based on SGOU SLM — Introduction to Information Technology (B21CA01DC). Covers Blocks 1–6, 24 Units, theory only.*  
*Prepared by Abdul Vahab A A | abdulvahabaa.in*
