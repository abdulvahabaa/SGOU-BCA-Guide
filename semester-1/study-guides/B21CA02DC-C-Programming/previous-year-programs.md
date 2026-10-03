# C Programming — Programs & Problems (Previous Year Papers)

**Subject:** Problem Solving and Programming in C (B21CA02DC)  
**Sources:** December 2024 | April 2025 | October 2025

> **Note:** Every **Question** below is copied **word-for-word** from [`question-bank.md`](question-bank.md).  
> Question numbers (Q6, Q63, Q117, etc.) are the **same** as in the full question bank. This file lists only **program, output, algorithm, and flowchart** PYQs — not all 117 questions.

---

## Exam section rules (quick reference)

| Section | Instruction | Marks each | How many to answer |
|---------|-------------|------------|-------------------|
| **A** | One word or one sentence | **1 mark** | Any **10** |
| **B** | Two or three sentences / short program | **2 marks** | Any **5** |
| **C** | One paragraph / program / algorithm | **4 marks** | Any **5** |
| **D** | Three pages (detailed) | **15 marks** | Any **2** |

---

# SECTION A — Output & Short Code (1 Mark Each)

*Answer any 10. Program-related questions below.*

---

## Q6 — 1 mark | December 2024

**Question (exact):** Predict the output of the following program:

```c
int main() {
    int i;
    for(i=0; i<25; i++);
    printf("%d", i);
    return 0;
}
```

**Answer:** `25`

**Why:** Semicolon after `for(...)` makes the loop body empty. Loop runs 25 times (i = 0 to 24), then i becomes 25. `printf` prints 25.


---

## Q19 — 1 mark | April 2025

**Question (exact):** What will be the value stored in variable 'a', `int a = 4.5 + 6.5;` ?

**Answer:** `a = 11`

**Why:** 4.5 + 6.5 = 11.0 (double). Assigned to `int a`, the decimal part is truncated → **11**.


---

## Q30 — 1 mark | April 2025

**Question (exact):** What will be the output?

```c
void main() {
    register x=10;
    printf("%d", &x);
}
```

**Answer:** **Compilation error**

**Why:** `register` variables cannot use address operator `&`. Compiler error.


---

## Q35 — 1 mark | October 2025

**Question (exact):** Write the output of the following code: `printf("%3d", 0);`

**Answer:** `  0` (0 printed with minimum width 3 — may show spaces before 0)

**Why:** `%3d` = integer with field width 3. Value 0 fits in 3 characters.


---

## Q21 — 1 mark | April 2025, October 2025 ⭐

**Question (exact):** What is the syntax of a for loop in C?

**Answer:**
```c
for(initialization; condition; update)
    statement;
```


---

## Q22 — 1 mark | April 2025

**Question (exact):** How do you declare an array of 20 integers in C?

**Answer:** `int arr[20];`


---

## Q36 — 1 mark | October 2025, December 2024 ⭐🔥

**Question (exact):** Give an example for a loop that tests condition at the bottom of the loop.

**Answer:**

```c
do {
    /* body executes at least once */
} while (condition);
```

**Example:** do-while loop — condition checked **after** the body (exit-controlled loop).

---

# SECTION B — Write Programs (2 Marks Each)

*Answer any 5. Full program questions below.*

---

## Q48 — 2 marks | December 2024, October 2025 ⭐

**Question (exact):** Write down the usage of the conditional operator.

**Answer:**

Syntax: `condition ? value_if_true : value_if_false`

```c
int a = 10, b = 20, max;
max = (a > b) ? a : b;   /* assigns larger value */
printf("Max = %d\n", max);
```

Used as shorthand for simple if-else assignment in one line.

---

## Q56 — 2 marks | April 2025

**Question (exact):** Write a C program to print a message.

**Answer:**

```c
#include <stdio.h>
int main() {
    printf("Hello, World!\n");
    return 0;
}
```


---

## Q60 — 2 marks | April 2025, December 2024 ⭐

**Question (exact):** Define one dimensional array with example.

**Answer:**

A **one-dimensional array** stores multiple values of the same type in a single row.

```c
int marks[5];              /* declaration */
int marks[5] = {10, 20, 30, 40, 50};   /* initialization */
printf("%d", marks[0]);  /* access first element → 10 */
```

---

## Q63 — 2 marks | April 2025, December 2024 ⭐🔥

**Question (exact):** Write a program to swap two numbers using call by reference.

**Answer:**

```c
#include <stdio.h>
void swap(int *a, int *b) {
    int t = *a;
    *a = *b;
    *b = t;
}
int main() {
    int x, y;
    printf("Enter two numbers: ");
    scanf("%d %d", &x, &y);
    printf("Before swap: x=%d, y=%d\n", x, y);
    swap(&x, &y);
    printf("After swap: x=%d, y=%d\n", x, y);
    return 0;
}
```


---

## Q65 — 2 marks | April 2025, December 2024, October 2025 ⭐🔥

**Question (exact):** What is the significance of argc and argv in command line arguments?

**Answer:**

- **argc** — argument count (includes program name)
- **argv** — array of strings; `argv[0]` = program name, `argv[1]`, `argv[2]` = user inputs
- Lets program read inputs at run time without recompiling

```c
int main(int argc, char *argv[]) {
    printf("Total args = %d\n", argc);
    printf("Program name = %s\n", argv[0]);
    return 0;
}
/* Run: ./prog hello  →  argc=2, argv[0]=./prog, argv[1]=hello */
```

---

## Q68 — 2 marks | October 2025, April 2025 ⭐🔥

**Question (exact):** Explain if—else if ladder.

**Answer:**

Tests multiple conditions **top to bottom**. First true condition runs; rest are skipped. Optional final `else` handles no match.

```c
int marks;
printf("Enter marks: ");
scanf("%d", &marks);
if(marks >= 90)
    printf("Grade A\n");
else if(marks >= 75)
    printf("Grade B\n");
else if(marks >= 60)
    printf("Grade C\n");
else
    printf("Fail\n");
```

---

## Q69 — 2 marks | October 2025

**Question (exact):** Write a program to print 1 to 10 using for loop.

**Answer:**

```c
#include <stdio.h>
int main() {
    int i;
    for(i = 1; i <= 10; i++)
        printf("%d ", i);
    return 0;
}
```


---

## Q70 — 2 marks | October 2025

**Question (exact):** Write a program to check whether a number is odd or even using user defined function.

**Answer:**

```c
#include <stdio.h>
int check(int n) {
    if(n % 2 == 0)
        return 1;   /* even */
    else
        return 0;   /* odd */
}
int main() {
    int n;
    printf("Enter a number: ");
    scanf("%d", &n);
    if(check(n))
        printf("%d is Even\n", n);
    else
        printf("%d is Odd\n", n);
    return 0;
}
```


---

## Q72 — 2 marks | October 2025

**Question (exact):** Write the output of the following code:

```c
void main() {
    printf("Hai");
    main();
    return 0;
}
```

**Answer:** Prints `Hai` repeatedly many times, then **stack overflow / program crash**.

**Why:** `main()` calls itself — infinite recursion with no base case.


---

# SECTION C — Programs, Algorithms, Flowcharts (4 Marks Each)

*Answer any 5. Program / algorithm / flowchart questions below.*

---

## Q78 — 4 marks | December 2024, October 2025 ⭐🔥

**Question (exact):** Explain entry-controlled loop and exit-controlled loop.

**Answer:**

| Type | When condition checked | Loops | Min runs |
|------|------------------------|-------|----------|
| **Entry-controlled** | Before body | for, while | 0 times |
| **Exit-controlled** | After body | do-while | 1 time |

**Entry-controlled (while):**
```c
while(i <= 10) {
    printf("%d ", i);
    i++;
}
```

**Exit-controlled (do-while):**
```c
do {
    printf("%d ", i);
    i++;
} while(i <= 10);
```

---

## Q80 — 4 marks | December 2024, October 2025, April 2025 ⭐🔥

**Question (exact):** Differentiate call by value and call by reference with example.

**Answer (theory + swap example):**

| Call by value | Call by reference |
|---------------|-------------------|
| Copy of value passed | Address passed using pointer |
| Original unchanged | Original changed |
| `func(a)` with `int x` | `func(&a)` with `int *x` |

```c
void swap(int *a, int *b) {
    int t = *a; *a = *b; *b = t;
}
/* main: swap(&x, &y); */
```


---

## Q86 — 4 marks | April 2025

**Question (exact):** Write an algorithm to find the sum of the first 100 natural numbers.

**Answer:**

```
1. START
2. SET sum = 0, i = 1
3. WHILE i <= 100 DO
       sum = sum + i
       i = i + 1
   END WHILE
4. PRINT sum
5. STOP
```

**Result:** sum = 5050


---

## Q89 — 4 marks | April 2025, October 2025 ⭐🔥

**Question (exact):** Write down the difference between break and continue statement.

**Answer:**

| break | continue |
|-------|----------|
| Exits loop/switch completely | Skips rest of current iteration only |
| Control goes after loop | Goes to next iteration |
| Used in switch to avoid fall-through | Used inside loops only |

```c
for(i = 1; i <= 5; i++) {
    if(i == 3) continue;   /* skip printing 3 */
    if(i == 5) break;      /* stop at 5 */
    printf("%d ", i);
}
/* Output: 1 2 4 */
```

---

## Q90 — 4 marks | April 2025, December 2024 ⭐🔥

**Question (exact):** Explain the functions malloc(), calloc(), realloc(), and free() in C with examples.

**Answer:**

| Function | Purpose |
|----------|---------|
| malloc(size) | Allocates memory; not initialized |
| calloc(n, size) | Allocates n blocks; initialized to 0 |
| realloc(ptr, size) | Resizes allocated memory |
| free(ptr) | Releases memory |

```c
#include <stdlib.h>
int *arr = (int*)malloc(5 * sizeof(int));
if(arr == NULL) { printf("Failed"); exit(1); }
arr[0] = 10;
free(arr);   /* always free after use */
```

---

## Q91 — 4 marks | April 2025

**Question (exact):** Write a program to find sum of squares of n natural numbers using do while loop.

**Answer:**

```c
#include <stdio.h>
int main() {
    int n, i = 1, sum = 0;
    printf("Enter n: ");
    scanf("%d", &n);
    do {
        sum = sum + (i * i);
        i++;
    } while(i <= n);
    printf("Sum of squares = %d\n", sum);
    return 0;
}
```


---

## Q93 — 4 marks | April 2025

**Question (exact):** Compare Structure and Union with example.

**Answer:**

| Feature | Structure | Union |
|---------|-----------|-------|
| Memory | Separate for each member | Shared by all members |
| Size | Sum of members | Largest member only |
| Members active | All at same time | One at a time |

```c
struct student {
    char name[20];
    int roll;
    float marks;
} s1;

union data {
    int i;
    float f;
} d;
d.i = 10;
d.f = 3.14;   /* overwrites i */
```

---

## Q95 — 4 marks | April 2025

**Question (exact):** Draw a flow chart to find biggest among two numbers.

**Answer (algorithm steps):**

```
START → Input A, B → Is A > B? 
  YES → Print A → STOP
  NO  → Print B → STOP
```

**Symbols:** Oval=Start/Stop | Parallelogram=Input | Diamond=Decision | Rectangle=Process


---

## Q96 — 4 marks | October 2025, December 2024 ⭐🔥

**Question (exact):** Explain type conversion with example.

**Answer:**

**Implicit conversion** — done automatically by compiler:
```c
int a = 3.7;        /* float → int, a = 3 */
float b = 5;        /* int → float, b = 5.0 */
```

**Explicit conversion (casting):**
```c
float result = (float)9 / 2;   /* result = 4.5 */
int x = 9 / 2;                 /* x = 4 (integer division) */
```

Converting larger type to smaller may lose data (truncation).

---

## Q97 — 4 marks | October 2025, December 2024 ⭐

**Question (exact):** Write a program to find the largest of three using conditional operator.

**Answer:**

```c
#include <stdio.h>
int main() {
    int a, b, c, max;
    printf("Enter three numbers: ");
    scanf("%d %d %d", &a, &b, &c);
    max = (a > b) ? ((a > c) ? a : c) : ((b > c) ? b : c);
    printf("Largest = %d\n", max);
    return 0;
}
```


---

## Q99 — 4 marks | October 2025

**Question (exact):** Write a program to print the positive difference between two numbers.

**Answer:**

```c
#include <stdio.h>
int main() {
    int a, b, diff;
    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);
    if(a > b)
        diff = a - b;
    else
        diff = b - a;
    printf("Positive difference = %d\n", diff);
    return 0;
}
```


---

## Q100 — 4 marks | October 2025, April 2025 ⭐🔥

**Question (exact):** Explain switch case with an example.

**Answer:**

```c
#include <stdio.h>
int main() {
    int choice;
    printf("Enter 1-Add, 2-Sub, 3-Mul: ");
    scanf("%d", &choice);
    switch(choice) {
        case 1: printf("Add selected\n"); break;
        case 2: printf("Sub selected\n"); break;
        case 3: printf("Mul selected\n"); break;
        default: printf("Invalid\n");
    }
    return 0;
}
```


---

## Q101 — 4 marks | October 2025

**Question (exact):** Explain the difference between break and continue with examples.

**Answer:**

**break** — exits the loop immediately:
```c
for(i = 1; i <= 10; i++) {
    if(i == 6) break;
    printf("%d ", i);
}
/* Output: 1 2 3 4 5 */
```

**continue** — skips current iteration, continues loop:
```c
for(i = 1; i <= 5; i++) {
    if(i == 3) continue;
    printf("%d ", i);
}
/* Output: 1 2 4 5 */
```

---

# SECTION D — Long Programs & Detailed Notes (15 Marks Each)

*Answer any 2. Program questions below.*

---

## Q106 — 15 marks | December 2024 🔥

**Question (exact):** Write a detailed note on the algorithm, flowchart, and symbols used in the flowchart with example.

**Answer:**

**Algorithm:** Step-by-step finite procedure to solve a problem.

**Example — find largest of two numbers:**
```
1. START
2. Input A, B
3. If A > B then Print A else Print B
4. STOP
```

**Flowchart symbols:**

| Symbol | Name | Use |
|--------|------|-----|
| Oval | Terminal | Start / Stop |
| Rectangle | Process | Calculation, assignment |
| Parallelogram | Input/Output | Read / Print |
| Diamond | Decision | if / condition |
| Arrow | Flow line | Direction of flow |

**Flow:** START → Input A,B → Is A>B? → YES: Print A → STOP | NO: Print B → STOP

---

## Q107 — 15 marks | December 2024, October 2025 ⭐🔥

**Question (exact):** Explain different loop control structures used in C programs with examples.

**Answer:** Explain **for**, **while**, **do-while** with syntax and one example each.

**for loop:**
```c
for(i = 1; i <= 5; i++)
    printf("%d ", i);
```

**while loop:**
```c
i = 1;
while(i <= 5) {
    printf("%d ", i);
    i++;
}
```

**do-while loop:**
```c
i = 1;
do {
    printf("%d ", i);
    i++;
} while(i <= 5);
```

| Loop | Type | Runs at least once? |
|------|------|---------------------|
| for | Entry-controlled | No |
| while | Entry-controlled | No |
| do-while | Exit-controlled | Yes |


---

## Q108 — 15 marks | December 2024, April 2025, October 2025 ⭐🔥

**Question (exact):** Explain recursion and its types with an example program.

**Answer:**

**Definition:** A function that calls itself. Must have **base case** (stop) and **recursive case**.

**Types:** Direct recursion (calls itself) | Indirect recursion (A calls B, B calls A)

**Example — Factorial:**

```c
#include <stdio.h>
int fact(int n) {
    if(n <= 1)          /* base case */
        return 1;
    return n * fact(n - 1);  /* recursive case */
}
int main() {
    int n = 5;
    printf("Factorial of %d = %d\n", n, fact(n));
    return 0;
}
```

**Output:** Factorial of 5 = 120


---

## Q109 — 15 marks | December 2024

**Question (exact):** Write a C program to read n array elements and sort in ascending order.

**Answer:**

```c
#include <stdio.h>
int main() {
    int n, a[100], i, j, temp;
    printf("Enter n: ");
    scanf("%d", &n);
    printf("Enter %d elements: ", n);
    for(i = 0; i < n; i++)
        scanf("%d", &a[i]);
    /* Bubble sort */
    for(i = 0; i < n-1; i++)
        for(j = 0; j < n-i-1; j++)
            if(a[j] > a[j+1]) {
                temp = a[j];
                a[j] = a[j+1];
                a[j+1] = temp;
            }
    printf("Sorted array: ");
    for(i = 0; i < n; i++)
        printf("%d ", a[i]);
    return 0;
}
```


---

## Q110 — 15 marks | April 2025, October 2025 ⭐🔥

**Question (exact):** Explain various operators used in C with example.

**Answer:**

| Type | Operators | Example |
|------|-----------|---------|
| Arithmetic | +, -, *, /, % | `9 % 2 = 1` |
| Relational | ==, !=, <, >, <=, >= | `a > b` |
| Logical | &&, \|\|, ! | `(a>0 && b>0)` |
| Assignment | =, +=, -= | `a += 5` |
| Increment | ++, -- | `i++` |
| Conditional | ? : | `max = (a>b)?a:b` |
| Bitwise | &, \|, ^, ~ | `a & b` |

```c
int a = 10, b = 3;
printf("Sum=%d Mod=%d\n", a+b, a%b);
printf("Max=%d\n", (a>b)?a:b);
```

---

## Q111 — 15 marks | April 2025, October 2025 ⭐🔥

**Question (exact):** Discuss about if-else-if ladder and switch statement with example.

**Answer:**

**if-else-if ladder** — multiple conditions tested in order:
```c
if(marks >= 90)      printf("A");
else if(marks >= 75) printf("B");
else if(marks >= 60) printf("C");
else                 printf("Fail");
```

**switch** — multi-way branch on single value:
```c
switch(choice) {
    case 1: printf("Add"); break;
    case 2: printf("Sub"); break;
    case 3: printf("Mul"); break;
    default: printf("Invalid");
}
```

Use if-else-if for ranges; switch for fixed values. Always use `break` in switch.

---

## Q112 — 15 marks | April 2025, December 2024 ⭐🔥

**Question (exact):** Discuss different types of arrays with examples, and write a program that demonstrates the use of a one-dimensional array to find the average of 10 numbers.

**Answer:**

**1D array:** `int arr[10];` — single row  
**2D array:** `int mat[3][4];` — rows and columns

**Program — Average of 10 numbers:**

```c
#include <stdio.h>
int main() {
    int arr[10], i;
    float sum = 0, avg;
    printf("Enter 10 numbers:\n");
    for(i = 0; i < 10; i++) {
        scanf("%d", &arr[i]);
        sum = sum + arr[i];
    }
    avg = sum / 10;
    printf("Average = %.2f\n", avg);
    return 0;
}
```


---

## Q113 — 15 marks | April 2025, December 2024, October 2025 ⭐🔥

**Question (exact):** Describe storage classes with examples.

**Answer:**

| Class | Scope | Lifetime | Default value |
|-------|-------|----------|---------------|
| auto | Block | Block | Garbage |
| register | Block | Block | Garbage |
| static | Block/File | Program | 0 |
| extern | Program | Program | 0 |

**auto** — default for local variables:
```c
void func() {
    int x;   /* auto by default */
}
```

**static** — retains value between calls:
```c
void counter() {
    static int count = 0;
    count++;
    printf("%d ", count);   /* prints 1, 2, 3 on each call */
}
```

**extern** — uses global variable defined elsewhere.

---

## Q116 — 15 marks | October 2025

**Question (exact):** Write a program to find the largest and second largest element in an array using function.

**Answer:**

```c
#include <stdio.h>
void findMax(int arr[], int n, int *max, int *second) {
    int i;
    *max = *second = arr[0];
    for(i = 1; i < n; i++) {
        if(arr[i] > *max) {
            *second = *max;
            *max = arr[i];
        } else if(arr[i] > *second && arr[i] != *max)
            *second = arr[i];
    }
}
int main() {
    int a[100], n, i, max, second;
    printf("Enter n: ");
    scanf("%d", &n);
    for(i = 0; i < n; i++)
        scanf("%d", &a[i]);
    findMax(a, n, &max, &second);
    printf("Largest = %d, Second largest = %d\n", max, second);
    return 0;
}
```


---

## Q117 — 15 marks | October 2025, April 2025 ⭐🔥

**Question (exact):** Write a program to implement file copy using command line arguments.

**Answer:**

```c
#include <stdio.h>
#include <stdlib.h>
int main(int argc, char *argv[]) {
    FILE *src, *dest;
    char ch;
    if(argc != 3) {
        printf("Usage: %s source dest\n", argv[0]);
        return 1;
    }
    src = fopen(argv[1], "r");
    dest = fopen(argv[2], "w");
    if(src == NULL || dest == NULL) {
        printf("Error opening file\n");
        return 1;
    }
    while((ch = fgetc(src)) != EOF)
        fputc(ch, dest);
    fclose(src);
    fclose(dest);
    printf("File copied successfully\n");
    return 0;
}
```

**Run:** `./copy source.txt dest.txt`

---

# MASTER TABLE — All Program-Related PYQs

*Exact question wording from [`question-bank.md`](question-bank.md)*

| Q# | Marks | Year(s) | Exact question (from paper) | Priority |
|----|-------|---------|----------------------------|----------|
| Q6 | 1 | Dec 2024 | Predict the output of the following program: | 🔥 |
| Q19 | 1 | Apr 2025 | What will be the value stored in variable 'a', `int a = 4.5 + 6.5;` ? | |
| Q21 | 1 | Apr 2025, Oct 2025 | What is the syntax of a for loop in C? | ⭐ |
| Q22 | 1 | Apr 2025 | How do you declare an array of 20 integers in C? | |
| Q30 | 1 | Apr 2025 | What will be the output? | 🔥 |
| Q35 | 1 | Oct 2025 | Write the output of the following code: `printf("%3d", 0);` | |
| Q36 | 1 | Oct 2025, Dec 2024 | Give an example for a loop that tests condition at the bottom of the loop. | ⭐🔥 |
| Q48 | 2 | Dec 2024, Oct 2025 | Write down the usage of the conditional operator. | ⭐ |
| Q56 | 2 | Apr 2025 | Write a C program to print a message. | |
| Q60 | 2 | Apr 2025, Dec 2024 | Define one dimensional array with example. | ⭐ |
| Q63 | 2 | Apr 2025, Dec 2024 | Write a program to swap two numbers using call by reference. | ⭐🔥 |
| Q65 | 2 | Apr 2025, Dec 2024, Oct 2025 | What is the significance of argc and argv in command line arguments? | ⭐🔥 |
| Q68 | 2 | Oct 2025, Apr 2025 | Explain if—else if ladder. | ⭐🔥 |
| Q69 | 2 | Oct 2025 | Write a program to print 1 to 10 using for loop. | |
| Q70 | 2 | Oct 2025 | Write a program to check whether a number is odd or even using user defined function. | |
| Q72 | 2 | Oct 2025 | Write the output of the following code: | 🔥 |
| Q78 | 4 | Dec 2024, Oct 2025 | Explain entry-controlled loop and exit-controlled loop. | ⭐🔥 |
| Q80 | 4 | Dec 2024, Oct 2025, Apr 2025 | Differentiate call by value and call by reference with example. | ⭐🔥 |
| Q86 | 4 | Apr 2025 | Write an algorithm to find the sum of the first 100 natural numbers. | |
| Q89 | 4 | Apr 2025, Oct 2025 | Write down the difference between break and continue statement. | ⭐🔥 |
| Q90 | 4 | Apr 2025, Dec 2024 | Explain the functions malloc(), calloc(), realloc(), and free() in C with examples. | ⭐🔥 |
| Q91 | 4 | Apr 2025 | Write a program to find sum of squares of n natural numbers using do while loop. | |
| Q93 | 4 | Apr 2025 | Compare Structure and Union with example. | |
| Q95 | 4 | Apr 2025 | Draw a flow chart to find biggest among two numbers. | |
| Q96 | 4 | Oct 2025, Dec 2024 | Explain type conversion with example. | ⭐🔥 |
| Q97 | 4 | Oct 2025, Dec 2024 | Write a program to find the largest of three using conditional operator. | ⭐ |
| Q99 | 4 | Oct 2025 | Write a program to print the positive difference between two numbers. | |
| Q100 | 4 | Oct 2025, Apr 2025 | Explain switch case with an example. | ⭐🔥 |
| Q101 | 4 | Oct 2025 | Explain the difference between break and continue with examples. | |
| Q106 | 15 | Dec 2024 | Write a detailed note on the algorithm, flowchart, and symbols used in the flowchart with example. | 🔥 |
| Q107 | 15 | Dec 2024, Oct 2025 | Explain different loop control structures used in C programs with examples. | ⭐🔥 |
| Q108 | 15 | Dec 2024, Apr 2025, Oct 2025 | Explain recursion and its types with an example program. | ⭐🔥 |
| Q109 | 15 | Dec 2024 | Write a C program to read n array elements and sort in ascending order. | |
| Q110 | 15 | Apr 2025, Oct 2025 | Explain various operators used in C with example. | ⭐🔥 |
| Q111 | 15 | Apr 2025, Oct 2025 | Discuss about if-else-if ladder and switch statement with example. | ⭐🔥 |
| Q112 | 15 | Apr 2025, Dec 2024 | Discuss different types of arrays with examples, and write a program that demonstrates the use of a one-dimensional array to find the average of 10 numbers. | ⭐🔥 |
| Q113 | 15 | Apr 2025, Dec 2024, Oct 2025 | Describe storage classes with examples. | ⭐🔥 |
| Q116 | 15 | Oct 2025 | Write a program to find the largest and second largest element in an array using function. | |
| Q117 | 15 | Oct 2025, Apr 2025 | Write a program to implement file copy using command line arguments. | ⭐🔥 |

---

**Wishing you all success in your semester exams.**

**Dua mein Yaad Rakhna.**
