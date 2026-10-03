# Computer Architecture and Operating Systems — For Exam Write-up

**Course:** B21CA03DC | **Coverage:** Blocks 1–6 (exam-likely portions only)

**Star meaning**

- ★★★ — 15 marks. Write definition + numbered points + diagram + 2-line conclusion.
- ★★ — 4 marks. Write 4 to 6 numbered points (or a small table).
- ★ — 1 or 2 marks. Write 2 to 4 lines only.

---

## Block 1: Basic Functional Architecture

### 1.1.1 Generations of Computers ★★

**For Exam**

Computer generations classify how hardware and software evolved. First generation used vacuum tubes (ENIAC, UNIVAC). Second used transistors and high-level languages like COBOL and FORTRAN. Third used integrated circuits, making systems smaller, faster and cheaper. Fourth used VLSI microprocessors and popularised personal computers. Fifth generation focuses on artificial intelligence. Across all generations, the basic von Neumann organisation of functional units remains the same.

**How to write (4 marks)**

Generations of computers describe how hardware technology and software capability changed over decades.

1. **First generation (1940–1956):** Vacuum tubes and magnetic drums. Machines were large, costly and power-hungry. Examples: UNIVAC, ENIAC, EDVAC.
2. **Second generation (1956–1963):** Transistors. Computers became smaller, faster and cooler. COBOL and FORTRAN appeared. Examples: IBM 1400 series, IBM 7090.
3. **Third generation (1964–1971):** Integrated Circuits (ICs). More reliable, faster, smaller and cheaper. Examples: IBM System/360, PDP-11.
4. **Fourth generation (1971–2010):** VLSI / microprocessors. Personal computers and laptops spread. Examples: Apple, CRAY-1.
5. **Fifth generation (present and future):** Artificial Intelligence. Systems that try to think and act like humans. Examples: PARAM 10000.

---

### 1.1.2 Functional Units of a Computer ★★★

**For Exam**

A basic computer has five functional units. The input unit brings data and programs into the system. Memory stores instructions, data and results. ALU performs arithmetic and logical operations. The control unit coordinates all activities by issuing control signals. The output unit presents results to the user. The CPU comprises ALU, control unit and registers. Units are linked by buses for data, address and control exchange.

**How to write (15 marks)**

**Introduction.** According to John von Neumann’s stored-program model, a computer has five main functional units that work together through buses: Input unit, Output unit, Memory unit, ALU, and Control unit. CPU = Control unit + ALU + Registers.

1. **Input unit:** Accepts data and programs from keyboard, mouse, scanner, disk, etc. and converts them into binary form.
2. **Memory unit:** Stores instructions, data, and intermediate/final results. Primary memory (RAM/ROM) is fast. Secondary memory (disk) is permanent and slower. Programs must reside in main memory during execution.
3. **ALU:** Performs arithmetic (+, −, ×, ÷) and logical/comparison operations. It is the computational work area of the CPU.
4. **Control unit:** Nerve centre of the computer. Fetches and interprets instructions, generates control signals and timing for all other units.
5. **Output unit:** Presents results to the user through monitor, printer, speaker, etc.

**How they work together:** Input brings programs/data into memory → Control unit sequences fetch–decode–execute → ALU processes operands → results go back to memory and then to output.

**Conclusion.** Each unit has a distinct role, but only their coordinated operation realises a complete computing system.

**Diagram to draw**

```
                    +------------------+
     Input  ------> |                  | ------> Output
    devices         |   MEMORY UNIT    |         devices
                    |  (programs+data) |
                    +--------+---------+
                             ^
                             | bus
                    +--------+---------+
                    |       CPU        |
                    |  ALU  |  CU      |
                    |     Registers    |
                    +------------------+
```

**1–2 mark line:** Memory unit stores **programs (instructions) and data**.

---

### 1.1.2.2 Primary and Secondary Memory ★★

**For Exam**

Memory stores code, data and results. Primary memory (ROM + RAM) is fast semiconductor storage; ROM is non-volatile firmware, RAM is volatile run-time memory. Secondary memory is cheaper, permanent and slower (disks) and supplements primary storage.

**How to write (4 marks)**

| Point | Primary memory | Secondary memory |
|-------|----------------|------------------|
| Speed | Fast | Slow |
| Cost | Expensive | Cheaper |
| Volatility | RAM is volatile; ROM is not | Non-volatile |
| Role | Programs must be here while running | Bulk permanent storage |
| Examples | RAM, ROM | Hard disk, optical disk |

---

### 1.1.2.3 ALU ★

**For Exam**

The ALU is the computational unit of the CPU. It performs arithmetic operations and logical/comparison operations. Results are sent to registers or memory.

**How to write (2 marks)**

ALU stands for Arithmetic and Logic Unit. It performs all arithmetic operations (+, −, ×, ÷) and logical operations (AND, OR, NOT, compare). It is the work area of the CPU.

---

### 1.1.2.4 Control Unit ★

**For Exam**

The control unit is the nerve centre. It fetches instructions, decodes them, and generates control signals to coordinate input, memory, ALU and output.

**How to write (1–2 marks)**

Primary function of the Control Unit: interpret instructions and generate control signals.

Two types of control signals: **timing signals** and **control signals** (for sequencing and execution).

---

### 1.1.3 Instruction Cycle ★

**For Exam**

Executing an instruction has phases: Fetch, Decode, Execute, and Store (write-back). The PC gives the address of the next instruction. IR holds the current instruction.

**How to write (2 marks)**

The various phases in executing an instruction are:

1. Fetch — instruction is taken from memory using PC.
2. Decode — opcode is interpreted.
3. Execute — ALU or data transfer is performed.
4. Store — result is written to register or memory.

---

### 1.1.4 Bus Structures and Bus Types ★★

**For Exam**

A bus is a shared set of lines for communication among CPU, memory and peripherals. The system bus has a bi-directional data bus, unidirectional address bus and control bus. Internal buses connect CPU internals; external buses connect peripherals. A single (common) bus structure is commonly used to connect I/O devices.

**How to write (2 marks) — Explain different bus types**

Buses interconnect units for exchange of data, address and control information.

1. **Internal (system) bus** — connects processor, memory and I/O.
2. **External bus** — connects peripherals such as keyboard and mouse to the CPU.

The system bus has three types of lines:

1. **Data bus** — bi-directional; carries data.
2. **Address bus** — unidirectional; carries addresses.
3. **Control bus** — read/write and other control signals.

Bus lines may also be **dedicated** or **multiplexed**.

**1 mark:** Usual BUS structure used to connect I/O devices = **Single bus / common bus structure**.

---

### 1.2.1 Registers, Decoder, Clock ★★

**For Exam**

Timing and control rely on flip-flops, registers, decoders, latches and a master clock. The clock synchronises all registers. Decoders convert opcodes into control signals. Registers hold addresses, data, instructions and status for fast CPU operation.

**How to write**

**What is used for synchronisation of digital devices? (1 mark)**  
Clock (clock pulses / master clock generator).

**What is the use of decoder? (2 marks)**  
A decoder translates encoded binary inputs into a specific output line or set of control signals. In the CPU it decodes the instruction opcode into control signals that direct ALU, registers and buses. It is also used for address decoding to select the correct memory or I/O device, and for converting sequence-counter outputs into timing signals (T0–T15).

**What is a register and mention the use of registers? (2 marks)**  
A register is a small, fast storage location inside the CPU made of flip-flops, holding binary data temporarily.

Uses:

- ACC — intermediate arithmetic results
- PC — address of next instruction
- IR — current instruction
- MAR — address of memory location
- MBR/DR — data buffer with memory
- SP — top of stack

**1 mark:** Register used to hold an address for the memory unit = **MAR**.  
**1 mark:** Program Counter (PC) keeps track of the **address of the next instruction**.  
**1 mark:** A 4-bit sequence counter can generate **16** timing signals (2⁴ = 16).

---

### 1.2.2 Hardwired and Microprogrammed Control ★★

**For Exam**

The timing and control unit generates timing and control signals for instruction execution. Hardwired control uses digital circuits (IR, decoders, sequence counter, logic gates) and is fast but inflexible. Microprogrammed control stores control words in ROM and is slower but easier to change.

**How to write (4 marks) — Key components of a hardwired control unit**

1. **Instruction Register (IR)** — holds the current instruction.
2. **Opcode decoder** (3×8 decoder) — decodes opcode into D0–D7.
3. **I-bit flip-flop** — stores the indirect-addressing bit.
4. **Sequence counter (SC)** — advances through timing states.
5. **Timing decoder** (4×16) — produces T0–T15.
6. **Control logic gates** — combine decoder, timing and IR bits to form final control signals.
7. **Master clock** — synchronises the sequence counter and registers.

Hardwired control is fast but inflexible.

**2 marks:** CMAR holds the **address of the next microinstruction** in control memory (ROM).

---

### 1.3.1 Addressing Modes — Need ★★

**For Exam**

Addressing modes specify how the CPU finds the operand(s) for an instruction — in the instruction itself, in a register, or in memory. They are needed for flexible, compact and efficient programming (pointers, loops, arrays, relocation, shorter address fields).

**How to write (4 marks)**

Addressing modes are methods of specifying the location of operands for CPU instructions. Their need/advantages are:

1. **Pointers** — refer to memory through address pointers.
2. **Loop control** — support counters so loops can step through data.
3. **Indexing** — access array/table elements using base + index.
4. **Program relocation** — programs can run from different starting addresses.
5. **Shorter instructions** — reduce bits in the address field.
6. **Efficiency and flexibility** — fewer instructions and better execution time.

---

### 1.3 Addressing Modes with Examples ★★★

**For Exam**

Addressing modes are ways of specifying operand locations. Implied mode hides the operand in the opcode. Immediate mode keeps data in the instruction. Direct mode gives the memory address. Register mode uses a CPU register. Register-indirect uses a register that holds the address. Auto-increment/decrement updates that register automatically. Indirect mode reads the address from memory. Indexed mode adds a base and an index register. These modes support pointers, loops, arrays, relocation and shorter instructions.

**How to write (15 marks)**

Addressing modes are ways of specifying operand locations for CPU instructions. Common modes are:

1. **Implied (Implicit) mode:** Operand is understood from the instruction itself (often accumulator). Examples: `CLC`, `INCA`, `NOP`.

2. **Immediate mode:** Actual operand is part of the instruction. Example: `MOV AX, 40H`; `ADD 07`. Useful for initialising registers.

3. **Direct addressing mode:** Instruction address field contains the memory address of the operand. EA = address field. Example: `LDA 2050`.

4. **Register mode:** Operand is in a CPU register named in the instruction. Example: `MOV EAX, EBX`; `ADD R1, R2`. Fast because no memory fetch is needed.

5. **Register indirect mode:** A register holds the effective address of the operand in memory. Example: `MOV A, M`. Saves address bits.

6. **Auto-increment / Auto-decrement mode:** Like register indirect, but the address register is automatically updated. Suited to sequential table access.

7. **Indirect addressing mode:** Instruction gives the address of a location that stores the effective address. Example: `ADD @200H` → AC ← AC + [[200H]]. Extra memory access.

8. **Indexed addressing mode:** EA = base address + index register content. Example: `MOV AX, [SI+05]`; `Load R4, 4(R2)`. Useful for arrays.

**Need:** addressing modes support pointers, loops, indexing, relocation, shorter address fields and efficient programming.

**Diagram to draw:** Instruction = [OPCODE][OPERAND / ADDRESS FIELD] → “How is operand located? → Addressing mode”.

---

### Direct vs Indirect ★★

**How to write (4 marks)**

| Point | Direct Addressing | Indirect Addressing |
|-------|-------------------|---------------------|
| Meaning | Address field contains the address of the operand | Address field gives a location that holds the effective address |
| Effective address | EA = address part of the instruction | EA = M[address field] |
| Memory references | One access | Extra access to get EA, then operand |
| Speed | Faster | Slower |
| Example | `LDA 2050` | `ADD @200H` |

**Summary:** In direct mode the instruction points straight to the operand; in indirect mode it points to a pointer.

---

### Indexed Addressing Mode ★★

**How to write (4 marks)**

In indexed addressing, the effective address is formed as **EA = base/displacement + contents of an index register**.

**Function:** The instruction provides a fixed base and names an index register. The CPU adds them to get the operand address. The base stays fixed while the index changes in a loop to visit array elements.

**Significance:** Ideal for arrays, tables and repetitive data access. Examples: `Load R4, 4(R2)`; `MOV AX, [SI+05]`. If base = 2800H and index = 01H, then EA = 2801H.

**1 mark:** Addressing mode that includes the operand as part of the instruction = **Immediate addressing mode**.

---

### 1.4 Program Control Instructions ★★

**For Exam**

Program control instructions change the PC and thus the flow of execution. They are needed for branching, loops, calls, halt and interrupts.

**How to write (2 marks) — Types of program control instructions**

The types of program control instructions are:

1. Unconditional branch / jump
2. Conditional branch
3. Subroutine call and return
4. Halt
5. Interrupt / skip instructions

**Unconditional branch (2 marks)**  
An unconditional branch always transfers control to a target address by loading a new value into the PC. Example: `JMP`. No flags are tested.

**Conditional branch (2 marks)**  
A conditional branch changes the PC only if a condition flag is true (zero, carry, etc.). Used for if-conditions and loops.

**What is a subroutine? (1 mark)**  
A subroutine is a named reusable procedure. It is invoked by a CALL, which saves the return address. RETURN restores the caller.

**HALT (1 mark)**  
When HALT is executed, the CPU stops fetching and executing instructions.

**NOP (2 marks)**  
NOP (No Operation) does nothing. It is used for timing delay or as a placeholder.

---

## Block 2: I/O and DMA

### 2.1 RTL ★

**For Exam**

RTL (Register Transfer Language) describes micro-operations and data transfers among registers, such as `R2 ← R1`.

**How to write**

**What does RTL stand for? (1 mark)**  
Register Transfer Language.

**RTL example (4 marks)**  
Transfer of data from register R1 to register R2 is written as:

`R2 ← R1`

This means the contents of R1 are copied to R2 in one clock pulse when the control signal is enabled.

**Fetch cycle (2 marks)**  
During fetch:

1. `MAR ← PC`
2. Memory is read; `IR ← M[MAR]`
3. `PC ← PC + 1`

**Role of multiplexer in a common bus (2 marks)**  
A multiplexer selects one register among many and places its contents on the common bus, using select control signals.

---

### 2.2 I/O Interface ★★ / ★★★

**For Exam**

An I/O interface links CPU and peripherals, handling data transfer, control, format conversion and synchronisation. Interfaces may be memory-mapped or isolated; transfer may use polling, interrupts or DMA.

**How to write (4 marks) — Functions of I/O interface**

The I/O interface mediates between the CPU and peripheral devices so they can communicate despite differences in speed, format and operation. Its main functions are:

1. **Data Transfer:** Moves data between the CPU and I/O devices through interface registers/ports.
2. **Control Signal Management:** Interprets control signals that start, stop and coordinate peripheral operations.
3. **Data Conversion:** Converts signal levels and data formats between electronic CPU/memory and electro-mechanical peripherals.
4. **Synchronisation:** Matches timing between fast CPU and slower devices so data is not lost (status checking, handshaking, buffering).

Without an interface, each peripheral’s different behaviour would make direct CPU connection impractical.

**What is polling? (2 marks)**  
Polling is a programmed I/O method in which the processor repeatedly checks the status flags of an I/O device to see whether it is ready. It is simple but wastes CPU time.

**Synchronous vs Asynchronous I/O (4 marks)**

| Point | Synchronous I/O | Asynchronous I/O |
|-------|-----------------|------------------|
| Timing | Common clock / fixed timing | Handshake / status signals |
| Speed match | When speeds are matched | When devices are slower or variable |
| Risk | Timing errors if clocking is wrong | Needs correct handshake |

**1 mark:** Two types of I/O interfaces = **Memory-mapped I/O** and **Isolated (port-mapped) I/O**.  
**1 mark:** Expansion of ASCII = **American Standard Code for Information Interchange**.  
**1 mark:** Bits in ASCII = **7 bits** (often stored as 8).

---

### 2.3 Priority Interrupts ★★

**For Exam**

A priority interrupt system ranks interrupt sources so the most urgent device is served first when requests arrive together. Priority may be set by software polling or by hardware (daisy chain or parallel encoder). Interrupts may be hardware or software, maskable or non-maskable.

**How to write (2 marks) — Priority interrupt**

A priority interrupt is an interrupt system that assigns priority levels to interrupt sources so that when two or more devices request service simultaneously, the **highest-priority request is recognised and serviced first**. High-speed devices (disk) get higher priority than slow devices (keyboard).

**How to write (4 marks) — Types of interrupts**

1. **Hardware interrupts:** Generated by external devices (e.g., key press).
   - **Maskable:** may be delayed when a higher-priority interrupt occurs.
   - **Non-maskable:** cannot be delayed; must be processed immediately.
2. **Software interrupts:** Generated by internal system/software activity.
   - **Normal software interrupts:** caused by software instructions (system calls).
   - **Exceptions:** unplanned interrupts (e.g., division by zero).

Priority interrupt hardware ranks simultaneous requests using daisy chain or parallel priority encoder.

**Diagram to draw**

```
 Device1 (High) ----\
 Device2            --> Priority logic --> CPU INT --> Save PC --> ISR --> Return
 Device3 (Low)  ----/
```

---

### 2.4 Direct Memory Access (DMA) ★★★

**For Exam**

DMA allows I/O devices to transfer data directly to/from memory using a DMA controller that temporarily becomes bus master. The CPU only sets up the transfer and is interrupted when done. Modes: burst, cycle stealing, transparent. Advantages: speed, less CPU overhead, high throughput for bulk transfers.

**How to write (15 marks)**

**Concept of DMA.**  
Direct Memory Access is a technique that allows peripheral devices to transfer data **directly to or from main memory without continuous involvement of the CPU** for each byte. A special hardware unit called the **DMA controller** manages addresses, word count and bus control.

**Need.** For high-speed devices (disk, network), moving large blocks under CPU program control is too slow and wasteful.

**Working.**

1. Device (or CPU setup) requests DMA.
2. DMA controller requests the system bus (**bus request**); CPU grants it (**bus grant**).
3. CPU initialises DMAC with starting memory address, number of words and transfer direction.
4. DMAC becomes **bus master** and transfers data between memory and I/O directly.
5. CPU can continue other instructions (depending on mode).
6. When count reaches zero, DMAC releases the bus and **interrupts** the CPU.

**DMA transfer modes.**

- **Burst mode:** bus held until whole block finishes.
- **Cycle stealing:** bus returned after each byte/word.
- **Transparent mode:** transfer only when CPU does not need the bus.

**Advantages.**

1. Efficient / high-speed transfer compared with programmed I/O.
2. CPU offloading — processor free for computation.
3. Higher throughput for bulk data.
4. Fewer interrupts — one completion interrupt per block.

**Conclusion.** DMA needs extra hardware, but for large transfers its performance benefits dominate.

**Diagram to draw**

```
  CPU ---- bus request/grant ---- DMA Controller ----> Memory
                                      ^
                                      |
                                   I/O Device
```

**1 mark:** DMA stands for **Direct Memory Access**.

---

## Block 3: Parallel Computer Structures

### 3.1 Parallel vs Serial ★

**For Exam**

Serial computing uses one processing element and executes one instruction at a time. Parallel computing uses many processing elements that work together on a problem at the same time.

**How to write (2 marks)**

| Point | Serial computing | Parallel computing |
|-------|------------------|--------------------|
| Processors | One PE | Many PEs |
| Execution | One instruction after another | Several operations overlap / run together |
| Speed | Slower for large problems | Faster for large problems |
| Example | Traditional uniprocessor | Multiprocessor, array processor |

**1 mark:** Several instructions executed simultaneously = **Parallel processing**.

---

### 3.2 Flynn’s Classification ★★★

**For Exam**

Flynn classifies computers by instruction-stream and data-stream multiplicity into SISD, SIMD, MISD and MIMD. SISD is the classic single-CPU von Neumann machine. SIMD uses one control unit and many PEs on different data. MISD feeds one data stream through multiple instruction streams (rare). MIMD runs multiple independent instruction and data streams (multiprocessors). Draw the 2×2 taxonomy and give one example for each.

**How to write (15 marks)**

**Introduction.** In 1966, Michael J. Flynn proposed a taxonomy based on the multiplicity of **instruction streams** and **data streams**. This gives four classes: SISD, SIMD, MISD and MIMD.

**Draw this table**

```
                    Instruction Stream
                 Single          Multiple
              +-------------+--------------+
    Single    |    SISD     |     MISD     |
 Data Stream  | (uniproces- | (rare)       |
              |  sor)       |              |
              +-------------+--------------+
    Multiple  |    SIMD     |     MIMD     |
              | (array /    | (multi-CPU)  |
              |  vector)    |              |
              +-------------+--------------+
```

1. **SISD (Single Instruction Single Data).** One CPU executes one instruction on one data item. Example: conventional PC.

2. **SIMD (Single Instruction Multiple Data).** One control unit broadcasts the same instruction to many processing elements, each on different data. Example: array processors, ILLIAC IV, GPU-style SIMD.

3. **MISD (Multiple Instruction Single Data).** Several processors execute different instructions on the same data stream. Rare in commercial machines.

4. **MIMD (Multiple Instruction Multiple Data).** Multiple processors run different programs on different data. Example: multiprocessors, multicore CPUs, clusters.

**Conclusion.** SISD is serial; SIMD and MIMD dominate practical parallel systems; MISD remains rare.

**1 mark:** SIMD stands for **Single Instruction Multiple Data**.  
**1 mark:** Uniprocessing computing devices are called **SISD** machines / uniprocessors.

---

### UMA vs NUMA ★★

**How to write (4 marks)**

| Point | UMA | NUMA |
|-------|-----|------|
| Memory view | All processors see shared memory with **equal access time** | Local memory is faster than remote |
| Typical system | SMP | Scalable multiprocessors |
| Scalability | Harder | Better |
| Programming | Simpler | More complex (locality matters) |

**Summary:** UMA offers equal memory latency (simpler, limited scale). NUMA makes local access faster than remote, improving scalability.

---

### 3.3 Pipelining ★★

**For Exam**

Pipelining overlaps stages of instruction execution so several instructions are in progress at once, increasing throughput. After fill time, completion rate approaches one instruction per cycle, subject to hazards.

**How to write (1 mark)**  
Pipelining is a technique in which the execution of multiple instructions is **overlapped**. Instruction processing is divided into stages (fetch, decode, execute, memory, write-back).

**How to write (4 marks) — What is pipelining? Define processor cycle**

**Pipelining** organises concurrent activity so that successive instructions overlap. Stages: Fetch → Decode → Execute → Memory → Write-back. After the pipeline fills, ideally one instruction completes every clock cycle.

A **processor cycle** is the time taken for a task to advance **one stage** — typically the slowest stage plus latch overhead. For a k-segment pipeline processing n tasks, total time ≈ **[k + (n − 1)] tp**.

**Need for Instruction Level Parallelism (4 marks)**

1. Higher performance from a single processor.
2. Better utilisation of CPU functional units.
3. Increased throughput — more instructions per unit time.
4. Exploitation of independent instructions.
5. Clock speed alone cannot keep raising performance, so ILP (pipelining, multiple issue) is needed.

**Pipeline bubble (2 marks)**  
A pipeline bubble is an empty stage cycle inserted when an instruction cannot advance (data hazard, branch, or structural conflict). That stage does no useful work, reducing throughput.

**True/False:** “Cycle time of the processor is reduced” is a disadvantage of pipelining. **False.** That is an advantage.

**Types of pipelining (2 marks):** Arithmetic pipeline, instruction pipeline, processor pipeline.

---

### 3.4 Vector Processing ★★

**For Exam**

Vector processing applies the same operation to a whole array/vector using vector registers and pipelined functional units. Performance is limited by setup and flushing times. Measures: improve vector instructions, batch similar scalar work, select vector-friendly algorithms, and use a vectorising compiler.

**How to write (1 mark)**  
Vector processing is processing in which the same operation is applied to a set of data (a vector/array) rather than to one scalar at a time.

**How to write (4 marks) — Performance measures of vector processing**

Vector processing performance depends on pipeline overheads.

**Overheads:** (i) **Setup time** — time to route the vector to the functional unit; (ii) **Flushing time** — time until the first result leaves the pipeline.

**Measures to improve performance:**

1. **Improve the vector instruction** — reduce memory accesses and maximise resource utilisation.
2. **Integrate scalar instructions** — group similar scalar instructions so the pipeline is not repeatedly reconfigured.
3. **Algorithm selection** — prefer algorithms that expose long vectors.
4. **Vectorising compiler** — recover parallelism from high-level code (A → L → O → M).

Sustained rate is often quoted in FLOPS/megaflops.

**1 mark:** Father of vector processing and supercomputing = **Seymour Cray**.

---

## Block 4: Basic Concepts of Operating Systems

### 4.1.1 Operating System — Definition and Components ★★

**For Exam**

OS hardware resources control ചെയ്യുകയും application programs convenient and safe ആയി run ചെയ്യാൻ അനുവദിക്കുകയും ചെയ്യുന്നു. OS components processes, memory, files, mass storage, I/O, protection/security എന്നിവ manage ചെയ്യുന്നു.

Write in exam English:

An operating system is a system program that controls computer resources and provides a platform for application programs. It is the interface between applications and hardware. OS itself does not do end-user tasks; it gives the environment for programs to do useful work.

**How to write (4 marks) — Process management**

Process management is the OS component that creates, schedules, terminates and coordinates processes.

1. Create/delete processes — allocate PCB, load program, assign PID.
2. Schedule CPU using long-term, short-term, medium-term schedulers and dispatcher.
3. Suspend/resume processes — ready, waiting, running; swapping if needed.
4. Provide synchronisation so shared data is not corrupted.
5. Provide IPC — pipes, messages, shared memory, sockets.
6. Handle termination and reclaim CPU, memory, open files.

A process is represented by a **PCB** (state, PC, registers, scheduling info, memory info).

---

### 4.1.3 Booting ★

**For Exam**

Booting is loading the OS into main memory when the computer starts. BIOS initialises hardware, finds the boot device, loads the boot loader/OS. Then OS loads drivers and starts the user environment.

**How to write**

**What is booting? (1 mark)**  
Booting is the process of starting the computer and loading the operating system into main memory.

**First program that runs? (1 mark)**  
**Bootstrap loader** / boot loader / bootstrap program.

**Booting process (2 marks)**  
Steps: BIOS/firmware initialises hardware and does POST; boot device is selected; boot sector/boot loader is loaded; loader loads OS kernel; OS loads device drivers and system processes; login/GUI is presented.

---

### 4.1.5 Types of Operating Systems ★★

**For Exam**

Types of OS as per SLM: serial processing, simple batch, multiprogrammed batch, time-sharing. Batch groups similar jobs; multiprogramming overlaps CPU work of several jobs; time-sharing shares CPU by time slices.

**How to write (2 marks)**  
Main types: (1) Serial Processing, (2) Simple Batch System, (3) Multiprogrammed Batch System, (4) Time-Sharing System.

**How to write (4 marks) — Time sharing OS**

A time-sharing OS is a multiprogramming system. CPU is shared among interactive users in short **time slices / quanta**. The short-term scheduler switches rapidly, so each user gets a responsive share.

Features: interactive response, multiple programs in memory, frequent context switches, fair CPU sharing.

Issues: reliability, security, integrity, communication.

---

### 4.1.6 Layered Structure of OS ★★

**For Exam**

OS structures: simple (MS-DOS — poor separation), layered (each level uses only lower levels; hardware layer 0, UI top), microkernel (Mach — minimal kernel, services as user modules, message communication). Layered design helps modularity and maintenance.

**How to write (4 marks)**

In the layered structure, the OS is divided into several levels/layers. **Layer 0 is hardware**. The highest layer **Layer N is the user interface**. Each layer has defined inputs, outputs and functions, and uses only the services of the layers below it.

**Advantages:** modularity, easier debugging/modification, clear abstraction. Lower layers hide hardware complexity.

Simple structure has less separation. Microkernel moves many services to user space.

**Diagram to draw**

```
 Layer N  = User interface
   ...
 Layer 1
 Layer 0  = Hardware
```

---

### 4.2 OS Services and System Calls ★

**For Exam**

OS services make program execution convenient: user interface, program execution, resource allocation, I/O, file-system manipulation, communication, error detection, accounting, protection and security.

**How to write (2 marks)**  
Different operating system services are: User Interface, Program execution, Resource allocation, I/O operations, File-system manipulation, Communication, Error detection, Accounting, Protection and security.

**fork() (2 marks)**  
`fork()` creates a new child process that is a copy of the parent. The child gets its own PID and PCB. After fork, both parent and child continue execution.

**Process-control system calls (2 marks)**  
`fork()` — create process; `exec()` — replace process image; `wait()` — parent waits for child; `exit()` — terminate process.

---

### 4.3 Process vs Program ★★

**For Exam**

A process is a program in execution. A program is a passive file on disk. A process is active and has state, PCB, registers and resources. Many processes can run from the same program.

**How to write (4 marks)**

| Aspect | Program | Process |
|--------|---------|---------|
| Nature | Passive entity | Dynamic / active entity |
| Storage | File on disk | Exists in main memory with resources |
| Definition | Set of instructions | A **program in execution** |
| Components | Code | Code + PC + registers + stack + data + state |
| Lifetime | Until the file is deleted | Created, scheduled, waits, then terminates |
| Multiplicity | One program file | Many processes from the same program |

Example: Word executable on disk is a program; each time you open Word, the OS creates a process.

---

### 4.3 Process State Diagram ★★★

**For Exam**

A process moves among New, Ready, Running, Waiting and Terminated. Only one process runs on a CPU at a time (per core); others wait in ready or device queues. The PCB stores all information needed to pause and resume a process.

**How to write (15 marks)**

**Introduction.** As a process executes, it changes **state**. The state reflects the current activity of the process. The process state diagram shows legal transitions among states.

**States.**

1. **New** — process is being created (OS allocates PCB and resources).
2. **Ready** — waiting to be assigned to a processor; sits in the ready queue.
3. **Running** — instructions are being executed on the CPU.
4. **Waiting (Blocked)** — waiting for an event (I/O completion); placed in a device queue.
5. **Terminated** — process has finished; OS reclaims resources.

**Transitions (must draw).**

- New → Ready: process is **admitted**.
- Ready → Running: **short-term scheduler** selects it; **dispatcher** context-switches.
- Running → Ready: **interrupt** or **time-slice expiry**.
- Running → Waiting: **I/O request** or event wait.
- Waiting → Ready: event/I/O **completes**.
- Running → Terminated: process **exits**.

**Context switch.** OS saves the old process’s state into its PCB and loads the new process’s PCB.

**Conclusion.** The diagram shows how the OS keeps the CPU busy by always having a ready process while others wait for I/O.

**Diagram to draw**

```
                 admit
        New ------------► Ready ◄------------+
                               │             │
                    dispatch   │             │ interrupt /
                               ▼             │ time-slice end
                            Running ---------+
                               │
                    I/O or     │     I/O or event
                    event wait │     completion
                               ▼
                            Waiting

        Running ──exit──► Terminated
```

**1 mark:** PCB stands for **Process Control Block**.  
**2 marks:** PC field in PCB stores the **address of the next instruction** of that process, used during context switch.  
**1 mark:** Name of a program in execution = **Process**.

---

### 4.3 Schedulers and Preemptive vs Non-preemptive ★★

**For Exam**

Schedulers decide which process runs when. Non-preemptive algorithms (FCFS, SJF) do not interrupt a running process for a higher-priority arrival; preemptive algorithms (SRTF, RR) can. Criteria: utilise CPU, maximise throughput, minimise TAT/WT/RT.

**How to write (4 marks) — Priority vs non-priority**

| Point | Non-priority (Non-preemptive) | Priority (Preemptive) |
|-------|-------------------------------|------------------------|
| Idea | Running process is not interrupted until it finishes or blocks | Scheduler may interrupt a low-priority process |
| Examples | FCFS, SJF | SRTF, Round Robin |
| Advantage | Simple; fewer context switches | Better response for urgent work |
| Disadvantage | Convoy effect; important jobs wait | More context switches; starvation |

**How to write (4 marks) — Preemptive vs non-preemptive**

| Point | Non-preemptive | Preemptive |
|-------|----------------|------------|
| Idea | Process keeps CPU until it finishes or blocks | Running process can be interrupted |
| When switch | Only on terminate or wait | Also on higher priority, shorter remaining time, or time quantum |
| Examples | FCFS, SJF | SRTF, Round Robin |
| Context switches | Fewer | More |
| Responsiveness | May delay short jobs | Better for interactive work |

**1 mark:** Scheduler invoked every time CPU needs a new process = **Short-term scheduler (CPU scheduler)**.  
**1 mark:** Scheduler that helps in swapping = **Medium-term scheduler**.

**Formulas to write in numerical answers**

- TAT = Completion Time − Arrival Time
- WT = TAT − Burst Time   **or**   WT = Start Time − Arrival Time
- Average WT = (sum of waiting times) / number of processes

---

### FCFS Numerical ★★★

**How to write (15 marks)**

FCFS schedules processes in order of **arrival time**. Non-preemptive.

**If given:** P1(0,4), P2(2,5), P3(3,3), P4(4,2), P5(5,1)

Order: P1 → P2 → P3 → P4 → P5

Gantt: P1: 0–4, P2: 4–9, P3: 9–12, P4: 12–14, P5: 14–15

WT = Start − AT: P1=0, P2=2, P3=6, P4=8, P5=9  
Average WT = 25/5 = **5**

Always draw the Gantt chart in the answer book.

---

### SJF Numerical ★★★

**How to write (15 marks)**

Non-preemptive SJF: among ready processes, choose the **smallest burst time**.

**If given:** P1(1,7), P2(2,5), P3(3,1), P4(4,2), P5(5,8)

- t=1 only P1 ready → P1 runs 1–8
- at t=8 ready: P2(5), P3(1), P4(2), P5(8) → shortest P3 → 8–9
- then P4 → 9–11
- then P2 → 11–16
- then P5 → 16–24

WT: P1=0, P2=9, P3=5, P4=5, P5=11  
Average WT = 30/5 = **6**

---

## Block 5: Process Synchronization

### 5.1 Interprocess Communication (IPC) ★★★

**For Exam**

IPC lets processes exchange data and synchronise. Main approaches are shared memory and message passing. Methods: pipes, named pipes (FIFO), message queues, semaphores, shared memory and sockets. Shared memory is fast but needs synchronisation; sockets suit networked client–server communication.

**How to write (4 marks)**

Interprocess communication (IPC) allows processes to exchange information and synchronise. Two main models are **shared memory** and **message passing**. Common methods:

1. **Pipes** — unidirectional flow between related processes.
2. **Named pipes (FIFO)** — bidirectional; even unrelated processes that know the name.
3. **Message queues** — messages stored until the receiver retrieves them.
4. **Shared memory** — fastest data exchange; needs semaphore/mutex.
5. **Semaphores** — integer synchronisers used with shared resources.
6. **Sockets** — client–server communication over a network.

**How to write (15 marks) — IPC methods + Dining Philosophers**

**Part A — IPC methods** (write the 6 methods above, each in 4–5 lines: what it is, who can use it, plus/minus).

**Part B — Dining Philosophers and deadlock**

Five philosophers sit around a table with five chopsticks. Each needs **two** chopsticks to eat.

**Deadlock:** If every philosopher picks up the **left** chopstick at once, each holds one and waits forever for the right one.

All four conditions hold:

- Mutual exclusion — a chopstick is held by at most one philosopher.
- Hold and wait — holds left while waiting for right.
- No preemption — chopsticks are not forcibly taken.
- Circular wait — P0 waits for P1 … P4 waits for P0.

**Solutions:** pick both chopsticks only if both free; odd/even different order; allow at most four philosophers to try at once.

**Draw:** five people in a circle with five chopsticks.

**1 mark:** IPC stands for **Inter-Process Communication**.

---

### 5.1.6 Mutual Exclusion ★

**For Exam**

Mutual exclusion means only one process may use a shared resource (critical section) at a time. Without it, concurrent updates cause race conditions. A correct solution must also ensure progress and bounded waiting.

**How to write (1 mark)**  
Mutual exclusion is a synchronisation principle that ensures if one process is using a shared variable or file (critical section), no other process can use that same shared resource at the same time.

---

### 5.3 Semaphores ★

**For Exam**

A semaphore is an integer synchronisation variable accessed only by atomic wait() and signal(). Binary semaphores provide mutual exclusion; counting semaphores manage limited resource pools.

**How to write**

**Two atomic operations (1 mark):** **wait()** and **signal()** (P and V).

**wait() (1 mark):** Decrements the semaphore; if the value would become negative, the process is **blocked**.

**signal() (1 mark):** Increments the semaphore and may **wake a waiting process**.

---

### 5.4 Deadlock ★★

**For Exam**

Deadlock occurs when processes wait indefinitely for resources held by each other. It arises only if mutual exclusion, hold-and-wait, no pre-emption and circular wait all hold. Breaking any one condition prevents deadlock.

**How to write (2 marks)**  
Deadlock is a situation in which a set of processes is permanently blocked because each process holds at least one resource and is waiting for a resource held by another process in the set, so none can proceed.

**Hold and wait (2 marks)**  
A process **holds at least one resource** while **waiting** to acquire additional resources held by others. Prevention: request all resources at once, or release held resources before requesting new ones.

**How to write (4 marks) — Deadlock with example**

Deadlock is permanent blocking of a set of processes. It occurs only when all four conditions hold: mutual exclusion, hold and wait, no preemption, and circular wait.

**Example:** P1 holds tape T and requests printer Pr. P2 holds printer Pr and requests tape T. Neither can finish → deadlock.

Another example: Dining Philosophers, if each picks one chopstick and waits for the second.

---

### 5.4 Banker's Algorithm ★★

**For Exam**

Banker’s algorithm is a deadlock-avoidance method. Processes declare maximum resource needs. Before granting a request, the OS checks whether the resulting allocation leaves a **safe state**. If yes, allocate; if not, the process waits.

**How to write (4 marks)**

Banker’s algorithm is a **deadlock-avoidance** technique for multiple instances of resource types. Each process declares its **maximum** need. The OS maintains Available, Max, Allocation and Need (Need = Max − Allocation).

When a process requests resources:

1. If Request ≤ Need, go to step 2; else **error**.
2. If Request ≤ Available, go to step 3; else **wait**.
3. **Tentatively allocate.**
4. Run **safety algorithm**. If a **safe sequence** exists, grant; else restore old state and wait.

Thus the system never enters an unsafe state — like a banker who never lends so much that remaining cash cannot cover customers’ maximum claims.

---

## Block 6: Memory Management and File Systems

### 6.1 Logical and Physical Address ★★

**For Exam**

The CPU generates a logical (virtual) address. The MMU maps it to a physical address in RAM using base and limit registers. Dynamic relocation: physical = logical + base (checked against limit).

**How to write (4 marks)**

| Point | Logical address space | Physical address space |
|-------|----------------------|------------------------|
| Generated by | CPU | Memory (after MMU translation) |
| Also called | Virtual address | Real / RAM address |
| Binding | Compile / load / execution time | Actual location in memory |
| Hardware | Seen by program | Mapped by **MMU** |

**1 mark:** MMU stands for **Memory Management Unit**.  
**1 mark:** Primary role of OS in memory management = keep track of memory, allocate/deallocate, decide what to move in/out.

---

### 6.1 Swapping ★

**For Exam**

Swapping is a memory management scheme in which a process is temporarily moved from main memory to secondary storage (swap space) so that memory becomes available for other processes; later it can be swapped back in.

**How to write (1 mark)**  
Swapping is temporarily moving a process from main memory to secondary memory (swap space) so that main memory can be made available for other processes, and later bringing it back when needed.

---

### 6.1 Contiguous Memory Allocation ★★

**For Exam**

In contiguous allocation a process occupies consecutive memory locations (fixed or dynamic partitions). Main disadvantages are **internal and external fragmentation**. Non-contiguous schemes like paging place process pieces in separate frames.

**How to write (1 mark)**  
Disadvantages of contiguous memory allocation: **internal fragmentation** and **external fragmentation**.

**Best-fit (4 marks)**  
Best-fit searches the list of free holes and allocates the **smallest hole that is large enough**. It tries to leave unused leftover as small as possible. Advantage: reduces wasted leftover in large holes. Disadvantage: leftover tiny holes may be unusable; searching takes time.

**Compaction (2 marks)**  
Compaction moves allocated blocks together so scattered free holes become one large free block. It reduces **external fragmentation**. Costly because processes must be relocated.

---

### 6.2 Paging ★★

**For Exam**

Paging is a non-contiguous scheme where processes are split into fixed-size pages and memory into frames. The page table maps logical page numbers to physical frames, so a process can be scattered in RAM without external fragmentation.

**How to write (2 marks) — Purpose of a page table**  
A page table maps each **logical page number** of a process to the **physical frame number** where that page resides in RAM. The MMU uses it to translate a logical address (page number + offset) into a physical address (frame number + offset).

---

### Page Fault ★

**How to write (1 mark)**  
A page fault is an exception/trap that occurs when a program tries to access a page that is mapped in its address space but is **not currently loaded in physical memory**.

**1 mark:** High paging activity = **Thrashing**.

---

### 6.2 Segmentation ★★

**For Exam**

Segmentation allocates memory in logical variable-sized segments (code, stack, modules). The segment table holds each segment’s base and length. MMU checks the offset against the limit and adds the base to form the physical address.

---

### 6.3 Virtual Memory and Demand Paging ★★

**For Exam**

Virtual memory maps a large logical address space onto smaller physical memory using demand paging. Pages are brought in only when needed; a missing page causes a page fault handled by the OS loading the page and resuming the process.

**How to write (2 marks) — How demand paging improves memory efficiency**

Demand paging loads a page into RAM **only when it is referenced**, instead of bringing the entire process at once.

1. Unused pages stay on disk, freeing frames.
2. More processes can be multiprogrammed.
3. Programs larger than physical memory can run.
4. Startup is faster.

**1 mark:** One technique used for virtual memory = **Demand paging**.

---

### 6.3 Page Replacement + Paging vs Segmentation ★★★

**For Exam**

Page replacement frees a frame when memory is full. FIFO replaces the oldest page; Optimal replaces the page not needed for the longest future time; LRU replaces the least recently used page. FIFO can show Belady’s anomaly.

**How to write (15 marks)**

**(a) Paging vs Segmentation**

| Point | Paging | Segmentation |
|-------|--------|--------------|
| Division | Fixed-size pages / frames | Variable-size logical segments |
| Address | (page number, offset) | (segment number, offset) |
| Table | Page table: page → frame | Segment table: base + limit |
| Fragmentation | No external; may have **internal** | No internal; may have **external** |
| User view | Invisible fixed blocks | Matches programmer’s modules |
| Sharing | Share pages | Share whole segments easily |

**(b) Page faults — method to write for any string**

1. Start with empty frames. First unique pages are all faults.
2. **FIFO:** replace the oldest page.
3. **Optimal:** replace the page used farthest in the future.
4. **LRU:** replace the least recently used page.
5. Count faults. Hits are not faults.

**Practised string (3 frames):** 9,2,3,4,1,2,3,5,1,0,5,9,9,0,1  
FIFO = **11**, Optimal = **8**, LRU = **12**.

Always draw the step table in the answer book.

---

### 6.4 File Allocation Methods ★★

**For Exam**

Disk space is allocated to files by contiguous, linked or indexed methods. Contiguous is simple and fast but fragments externally; linked avoids external fragmentation but hurts random access; indexed collects pointers in an index block to support direct access with some pointer overhead.

**How to write (4 marks)**

**1. Contiguous allocation** — file occupies consecutive disk blocks; directory stores start + length.  
- Advantages: simple; excellent sequential and direct access; fast.  
- Disadvantages: external fragmentation; must often declare size at creation.

**2. Linked allocation** — file is a linked list of blocks; directory points to first block.  
- Advantages: no external fragmentation; file can grow easily.  
- Disadvantages: pointer overhead; mainly sequential access; pointer loss can truncate file.

**3. Indexed allocation** — all block addresses collected in an **index block**; directory points to the index.  
- Advantages: direct access; no external fragmentation; flexible growth.  
- Disadvantages: index-block overhead; large files may need multilevel index.

---

## How to present any long answer in the booklet

1. Start with a **2-line definition**.
2. Write **numbered points** (not one long paragraph).
3. Draw the **diagram** and label it.
4. End with a **2-line conclusion**.

That is the writing pattern used in the SLM model answers and in last year’s paper.
)
