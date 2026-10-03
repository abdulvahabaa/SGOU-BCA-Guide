# Lab Record Template

SREENARAYANAGURU OPEN UNIVERSITY

## B21CA04DC DATA STRUCTURES — Lab Record

---

# INDEX

| Sl.No | Date | Name of Experiment | Page No | Signature |
| --- | --- | --- | --- | --- |
| 1 | 12/04/2026 | Insertion of Elements in an Array |  |  |
| 2 | 12/04/2026 | Deletion of Elements in an Array |  |  |
| 3 | 12/04/2026 | Linear Search |  |  |
| 4 | 12/04/2026 | Creation, Insertion and Display of Linked List |  |  |
| 5 | 12/04/2026 | Queue Operations Using Array |  |  |
| 6 | 07/06/2026 | Queue Operations Using Linked List |  |  |
| 7 | 07/06/2026 | Stack Operations Using Array |  |  |
| 8 | 07/06/2026 | Stack Operations Using Linked List |  |  |
| 9 | 07/06/2026 | Insertion Sort |  |  |
| 10 | 07/06/2026 | Selection Sort |  |  |
| 11 | 14/06/2026 | Bubble Sort |  |  |
| 12 | 14/06/2026 | Binary Search |  |  |
| 13 | 14/06/2026 | Quick Sort |  |  |
| 14 | 14/06/2026 | Matrix Addition Using Array |  |  |
| 15 | 14/06/2026 | Sum of Elements of an Array |  |  |

---

## Experiment 1: Insertion of Elements in an Array

**Date:** 12/04/2026

**Aim:** To write a C program to insert an element at a given position in an array.

**Algorithm:**

1. Start
2. Read the number of elements n
3. Read n elements into array arr[]
4. Read the position (pos) where element is to be inserted
5. Read the element (item) to be inserted
6. Start from last element, shift each element one position to right
7. Continue shifting until position pos is reached
8. Place item at arr[pos-1]
9. Increase n by 1
10. Print all elements of updated array
11. Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>
void main() {
    int arr[100], n, i, pos, item;
    clrscr();
    printf("Enter number of elements: ");
    scanf("%d", &n);
    for(i = 0; i < n; i++)
        scanf("%d", &arr[i]);
    printf("Enter position: ");
    scanf("%d", &pos);
    printf("Enter element: ");
    scanf("%d", &item);
    for(i = n; i >= pos; i--)
        arr[i] = arr[i-1];
    arr[pos-1] = item;
    n++;
    printf("After insertion: ");
    for(i = 0; i < n; i++)
        printf("%d ", arr[i]);
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Enter number of elements: 4
10 20 30 40
Enter position: 2
Enter element: 15
After insertion: 10 15 20 30 40
```

---

## Experiment 2: Deletion of Elements in an Array

**Date:** 12/04/2026

**Aim:** To write a C program to delete an element from a given position in an array.

**Algorithm:**

1. Start
2. Read the number of elements n
3. Read n elements into array arr[]
4. Read the position (pos) to delete
5. Store the element at arr[pos-1] in item
6. Start from position pos, shift each element one position to left
7. Continue shifting until last element
8. Decrease n by 1
9. Print deleted element
10. Print all elements of updated array
11. Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>
void main() {
    int arr[100], n, i, pos, item;
    clrscr();
    printf("Enter number of elements: ");
    scanf("%d", &n);
    for(i = 0; i < n; i++)
        scanf("%d", &arr[i]);
    printf("Enter position to delete: ");
    scanf("%d", &pos);
    item = arr[pos-1];
    for(i = pos-1; i < n-1; i++)
        arr[i] = arr[i+1];
    n--;
    printf("Deleted element: %d\n", item);
    printf("After deletion: ");
    for(i = 0; i < n; i++)
        printf("%d ", arr[i]);
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Enter number of elements: 5
10 20 30 40 50
Enter position to delete: 3
Deleted element: 30
After deletion: 10 20 40 50
```

---

## Experiment 3: Linear Search

**Date:** 12/04/2026

**Aim:** To write a C program to search an element in an array using Linear Search.

**Algorithm:**

1. Start
2. Read the number of elements n
3. Read n elements into array arr[]
4. Read the element to search (key)
5. Set i = 0 and found = 0
6. Compare key with arr[i]
7. If arr[i] == key, print position (i+1), set found = 1 and stop loop
8. If not equal, increment i by 1
9. Repeat steps 6 to 8 until i reaches n
10. If found == 0, print "Element not found"
11. Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>
void main() {
    int arr[100], n, i, key, found = 0;
    clrscr();
    printf("Enter number of elements: ");
    scanf("%d", &n);
    for(i = 0; i < n; i++)
        scanf("%d", &arr[i]);
    printf("Enter element to search: ");
    scanf("%d", &key);
    for(i = 0; i < n; i++) {
        if(arr[i] == key) {
            printf("Found at position %d", i+1);
            found = 1;
            break;
        }
    }
    if(found == 0)
        printf("Element not found");
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Enter number of elements: 5
10 20 30 40 50
Enter element to search: 30
Found at position 3
```

---

## Experiment 4: Creation, Insertion and Display of Linked List

**Date:** 12/04/2026

**Aim:** To write a C program to create a linked list, insert a node at beginning and display it.

**Algorithm:**

**Creation:**

1. Start
2. Read number of nodes n
3. Create a new node using malloc
4. Read data into new node, set next = NULL
5. If head == NULL, set head = newnode
6. Else traverse to last node and link newnode to it
7. Repeat steps 3 to 6 for all n nodes
8. Stop

**Insertion at Beginning:**

1. Start
2. Create a new node using malloc
3. Read data into new node
4. Set newnode->next = head
5. Update head = newnode
6. Stop

**Display:**

1. Start
2. Set temp = head
3. If temp == NULL, print "List is empty" and stop
4. Print temp->data
5. Move temp = temp->next
6. Repeat steps 4 and 5 until temp == NULL
7. Print NULL and Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>
#include<alloc.h>

struct node {
    int data;
    struct node *next;
};
struct node *head = NULL;

void create(int n) {
    int i;
    struct node *temp, *newnode;
    for(i = 0; i < n; i++) {
        newnode = (struct node*)malloc(sizeof(struct node));
        printf("Enter data: ");
        scanf("%d", &newnode->data);
        newnode->next = NULL;
        if(head == NULL) {
            head = newnode;
        } else {
            temp = head;
            while(temp->next != NULL)
                temp = temp->next;
            temp->next = newnode;
        }
    }
}

void insert_begin() {
    struct node *newnode;
    newnode = (struct node*)malloc(sizeof(struct node));
    printf("Enter data to insert: ");
    scanf("%d", &newnode->data);
    newnode->next = head;
    head = newnode;
}

void display() {
    struct node *temp = head;
    printf("List: ");
    while(temp != NULL) {
        printf("%d -> ", temp->data);
        temp = temp->next;
    }
    printf("NULL\n");
}

void main() {
    int n;
    clrscr();
    printf("Enter number of nodes: ");
    scanf("%d", &n);
    create(n);
    display();
    insert_begin();
    display();
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Enter number of nodes: 3
Enter data: 10
Enter data: 20
Enter data: 30
List: 10 -> 20 -> 30 -> NULL
Enter data to insert: 5
List: 5 -> 10 -> 20 -> 30 -> NULL
```

---

## Experiment 5: Queue Operations Using Array

**Date:** 12/04/2026

**Aim:** To write a C program to implement Enqueue, Dequeue and Display of Queue using Array.

**Algorithm:**

**Enqueue:**

1. Start
2. Check if rear == MAX-1, if yes print "Queue Overflow" and stop
3. If front == -1, set front = 0
4. Increment rear by 1
5. Insert element at queue[rear]
6. Print inserted element
7. Stop

**Dequeue:**

1. Start
2. Check if front == -1 or front > rear, if yes print "Queue Underflow" and stop
3. Print element at queue[front]
4. Increment front by 1
5. Stop

**Display:**

1. Start
2. Check if queue is empty, if yes print "Queue is empty" and stop
3. Print all elements from front to rear one by one
4. Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>
#define MAX 5

int queue[MAX], front = -1, rear = -1;

void enqueue(int value) {
    if(rear == MAX-1) {
        printf("Queue Overflow\n");
    } else {
        if(front == -1) front = 0;
        rear++;
        queue[rear] = value;
        printf("Inserted: %d\n", value);
    }
}

void dequeue() {
    if(front == -1 || front > rear) {
        printf("Queue Underflow\n");
    } else {
        printf("Deleted: %d\n", queue[front]);
        front++;
    }
}

void display() {
    int i;
    if(front == -1 || front > rear) {
        printf("Queue is empty\n");
    } else {
        printf("Queue: ");
        for(i = front; i <= rear; i++)
            printf("%d ", queue[i]);
        printf("\n");
    }
}

void main() {
    clrscr();
    enqueue(10);
    enqueue(20);
    enqueue(30);
    display();
    dequeue();
    display();
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Inserted: 10
Inserted: 20
Inserted: 30
Queue: 10 20 30
Deleted: 10
Queue: 20 30
```

---

## Experiment 6: Queue Operations Using Linked List

**Date:** 07/06/2026

**Aim:** To write a C program to implement Enqueue, Dequeue and Display of Queue using Linked List.

**Algorithm:**

**Enqueue:**

1. Start
2. Create a new node using malloc
3. Read data into new node, set newnode->next = NULL
4. If front == NULL, set front = rear = newnode
5. Else set rear->next = newnode and update rear = newnode
6. Print inserted element
7. Stop

**Dequeue:**

1. Start
2. If front == NULL, print "Queue Underflow" and stop
3. Store temp = front
4. Print temp->data
5. Move front = front->next
6. If front == NULL, set rear = NULL
7. Free temp
8. Stop

**Display:**

1. Start
2. If front == NULL, print "Queue is empty" and stop
3. Set temp = front
4. Print temp->data followed by "->"
5. Move temp = temp->next
6. Repeat steps 4 and 5 until temp == NULL
7. Print NULL and Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>
#include<alloc.h>

struct node {
    int data;
    struct node *next;
};
struct node *front = NULL, *rear = NULL;

void enqueue(int value) {
    struct node *newnode;
    newnode = (struct node*)malloc(sizeof(struct node));
    newnode->data = value;
    newnode->next = NULL;
    if(front == NULL) {
        front = rear = newnode;
    } else {
        rear->next = newnode;
        rear = newnode;
    }
    printf("Inserted: %d\n", value);
}

void dequeue() {
    struct node *temp;
    if(front == NULL) {
        printf("Queue Underflow\n");
        return;
    }
    temp = front;
    printf("Deleted: %d\n", temp->data);
    front = front->next;
    if(front == NULL) rear = NULL;
    free(temp);
}

void display() {
    struct node *temp = front;
    if(front == NULL) {
        printf("Queue is empty\n");
        return;
    }
    printf("Queue: ");
    while(temp != NULL) {
        printf("%d -> ", temp->data);
        temp = temp->next;
    }
    printf("NULL\n");
}

void main() {
    clrscr();
    enqueue(10);
    enqueue(20);
    enqueue(30);
    display();
    dequeue();
    display();
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Inserted: 10
Inserted: 20
Inserted: 30
Queue: 10 -> 20 -> 30 -> NULL
Deleted: 10
Queue: 20 -> 30 -> NULL
```

---

## Experiment 7: Stack Operations Using Array

**Date:** 07/06/2026

**Aim:** To write a C program to implement Push, Pop and Display of Stack using Array.

**Algorithm:**

**Push:**

1. Start
2. Check if top == MAX-1, if yes print "Stack Overflow" and stop
3. Increment top by 1
4. Insert element at stack[top]
5. Print inserted element
6. Stop

**Pop:**

1. Start
2. Check if top == -1, if yes print "Stack Underflow" and stop
3. Print element at stack[top]
4. Decrement top by 1
5. Stop

**Display:**

1. Start
2. Check if top == -1, if yes print "Stack is empty" and stop
3. Print elements from stack[top] to stack[0] one by one
4. Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>
#define MAX 5

int stack[MAX], top = -1;

void push(int value) {
    if(top == MAX-1) {
        printf("Stack Overflow\n");
    } else {
        top++;
        stack[top] = value;
        printf("Inserted: %d\n", value);
    }
}

void pop() {
    if(top == -1) {
        printf("Stack Underflow\n");
    } else {
        printf("Deleted: %d\n", stack[top]);
        top--;
    }
}

void display() {
    int i;
    if(top == -1) {
        printf("Stack is empty\n");
    } else {
        printf("Stack: ");
        for(i = top; i >= 0; i--)
            printf("%d ", stack[i]);
        printf("\n");
    }
}

void main() {
    clrscr();
    push(10);
    push(20);
    push(30);
    display();
    pop();
    display();
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Inserted: 10
Inserted: 20
Inserted: 30
Stack: 30 20 10
Deleted: 30
Stack: 20 10
```

---

## Experiment 8: Stack Operations Using Linked List

**Date:** 07/06/2026

**Aim:** To write a C program to implement Push, Pop and Display of Stack using Linked List.

**Algorithm:**

**Push:**

1. Start
2. Create a new node using malloc
3. Read data into new node
4. Set newnode->next = top
5. Update top = newnode
6. Print inserted element
7. Stop

**Pop:**

1. Start
2. If top == NULL, print "Stack Underflow" and stop
3. Store temp = top
4. Print temp->data
5. Move top = top->next
6. Free temp
7. Stop

**Display:**

1. Start
2. If top == NULL, print "Stack is empty" and stop
3. Set temp = top
4. Print temp->data followed by "->"
5. Move temp = temp->next
6. Repeat steps 4 and 5 until temp == NULL
7. Print NULL and Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>
#include<alloc.h>

struct node {
    int data;
    struct node *next;
};
struct node *top = NULL;

void push(int value) {
    struct node *newnode;
    newnode = (struct node*)malloc(sizeof(struct node));
    newnode->data = value;
    newnode->next = top;
    top = newnode;
    printf("Inserted: %d\n", value);
}

void pop() {
    struct node *temp;
    if(top == NULL) {
        printf("Stack Underflow\n");
        return;
    }
    temp = top;
    printf("Deleted: %d\n", temp->data);
    top = top->next;
    free(temp);
}

void display() {
    struct node *temp = top;
    if(top == NULL) {
        printf("Stack is empty\n");
        return;
    }
    printf("Stack: ");
    while(temp != NULL) {
        printf("%d -> ", temp->data);
        temp = temp->next;
    }
    printf("NULL\n");
}

void main() {
    clrscr();
    push(10);
    push(20);
    push(30);
    display();
    pop();
    display();
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Inserted: 10
Inserted: 20
Inserted: 30
Stack: 30 -> 20 -> 10 -> NULL
Deleted: 30
Stack: 20 -> 10 -> NULL
```

---

## Experiment 9: Insertion Sort

**Date:** 07/06/2026

**Aim:** To write a C program to sort an array using Insertion Sort.

**Algorithm:**

1. Start
2. Read the number of elements n
3. Read n elements into array arr[]
4. For i = 1 to n-1, repeat steps 5 to 7
5. Set key = arr[i] and j = i-1
6. While j >= 0 and arr[j] > key, shift arr[j] to arr[j+1] and decrement j
7. Place key at arr[j+1]
8. Print sorted array
9. Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>

void main() {
    int arr[100], n, i, j, key;
    clrscr();
    printf("Enter number of elements: ");
    scanf("%d", &n);
    printf("Enter elements: ");
    for(i = 0; i < n; i++)
        scanf("%d", &arr[i]);
    for(i = 1; i < n; i++) {
        key = arr[i];
        j = i - 1;
        while(j >= 0 && arr[j] > key) {
            arr[j+1] = arr[j];
            j--;
        }
        arr[j+1] = key;
    }
    printf("Sorted array: ");
    for(i = 0; i < n; i++)
        printf("%d ", arr[i]);
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Enter number of elements: 5
Enter elements: 40 10 30 20 50
Sorted array: 10 20 30 40 50
```

---

## Experiment 10: Selection Sort

**Date:** 07/06/2026

**Aim:** To write a C program to sort an array using Selection Sort.

**Algorithm:**

1. Start
2. Read the number of elements n
3. Read n elements into array arr[]
4. For i = 0 to n-2, repeat steps 5 to 7
5. Set min = i
6. For j = i+1 to n-1, if arr[j] < arr[min], set min = j
7. Swap arr[i] and arr[min]
8. Print sorted array
9. Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>

void main() {
    int arr[100], n, i, j, min, temp;
    clrscr();
    printf("Enter number of elements: ");
    scanf("%d", &n);
    printf("Enter elements: ");
    for(i = 0; i < n; i++)
        scanf("%d", &arr[i]);
    for(i = 0; i < n-1; i++) {
        min = i;
        for(j = i+1; j < n; j++) {
            if(arr[j] < arr[min])
                min = j;
        }
        temp = arr[i];
        arr[i] = arr[min];
        arr[min] = temp;
    }
    printf("Sorted array: ");
    for(i = 0; i < n; i++)
        printf("%d ", arr[i]);
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Enter number of elements: 5
Enter elements: 40 10 30 20 50
Sorted array: 10 20 30 40 50
```

---

## Experiment 11: Bubble Sort

**Date:** 14/06/2026

**Aim:** To write a C program to sort an array using Bubble Sort.

**Algorithm:**

1. Start
2. Read the number of elements n
3. Read n elements into array arr[]
4. For i = 0 to n-2, repeat steps 5 to 6
5. For j = 0 to n-i-2
6. If arr[j] > arr[j+1], swap arr[j] and arr[j+1]
7. Print sorted array
8. Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>

void main() {
    int arr[100], n, i, j, temp;
    clrscr();
    printf("Enter number of elements: ");
    scanf("%d", &n);
    printf("Enter elements: ");
    for(i = 0; i < n; i++)
        scanf("%d", &arr[i]);
    for(i = 0; i < n-1; i++) {
        for(j = 0; j < n-i-1; j++) {
            if(arr[j] > arr[j+1]) {
                temp = arr[j];
                arr[j] = arr[j+1];
                arr[j+1] = temp;
            }
        }
    }
    printf("Sorted array: ");
    for(i = 0; i < n; i++)
        printf("%d ", arr[i]);
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Enter number of elements: 5
Enter elements: 40 10 30 20 50
Sorted array: 10 20 30 40 50
```

---

## Experiment 12: Binary Search

**Date:** 14/06/2026

**Aim:** To write a C program to search an element in a sorted array using Binary Search.

**Algorithm:**

1. Start
2. Read the number of elements n
3. Read n sorted elements into array arr[]
4. Read the element to search (key)
5. Set low = 0, high = n-1, found = 0
6. While low <= high, repeat steps 7 to 10
7. Set mid = (low + high) / 2
8. If arr[mid] == key, print position (mid+1), set found = 1 and stop loop
9. If arr[mid] < key, set low = mid + 1
10. Else set high = mid - 1
11. If found == 0, print "Element not found"
12. Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>

void main() {
    int arr[100], n, i, key, low, high, mid, found = 0;
    clrscr();
    printf("Enter number of elements: ");
    scanf("%d", &n);
    printf("Enter sorted elements: ");
    for(i = 0; i < n; i++)
        scanf("%d", &arr[i]);
    printf("Enter element to search: ");
    scanf("%d", &key);
    low = 0;
    high = n - 1;
    while(low <= high) {
        mid = (low + high) / 2;
        if(arr[mid] == key) {
            printf("Found at position %d", mid+1);
            found = 1;
            break;
        } else if(arr[mid] < key) {
            low = mid + 1;
        } else {
            high = mid - 1;
        }
    }
    if(found == 0)
        printf("Element not found");
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Enter number of elements: 5
Enter sorted elements: 10 20 30 40 50
Enter element to search: 30
Found at position 3
```

---

## Experiment 13: Quick Sort

**Date:** 14/06/2026

**Aim:** To write a C program to sort an array using Quick Sort.

**Algorithm:**

1. Start
2. Read the number of elements n
3. Read n elements into array arr[]
4. Call quicksort(arr, 0, n-1)
5. In quicksort: if low >= high, return
6. Choose pivot = arr[high]
7. Partition array: place elements less than pivot to left, greater to right
8. Place pivot at correct position
9. Recursively sort left and right parts
10. Print sorted array
11. Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>

int partition(int arr[], int low, int high) {
    int pivot = arr[high];
    int i = low - 1, j, temp;
    for(j = low; j < high; j++) {
        if(arr[j] <= pivot) {
            i++;
            temp = arr[i]; arr[i] = arr[j]; arr[j] = temp;
        }
    }
    temp = arr[i+1]; arr[i+1] = arr[high]; arr[high] = temp;
    return i + 1;
}

void quicksort(int arr[], int low, int high) {
    int pi;
    if(low < high) {
        pi = partition(arr, low, high);
        quicksort(arr, low, pi - 1);
        quicksort(arr, pi + 1, high);
    }
}

void main() {
    int arr[100], n, i;
    clrscr();
    printf("Enter number of elements: ");
    scanf("%d", &n);
    printf("Enter elements: ");
    for(i = 0; i < n; i++)
        scanf("%d", &arr[i]);
    quicksort(arr, 0, n-1);
    printf("Sorted array: ");
    for(i = 0; i < n; i++)
        printf("%d ", arr[i]);
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Enter number of elements: 5
Enter elements: 40 10 30 20 50
Sorted array: 10 20 30 40 50
```

---

## Experiment 14: Matrix Addition Using Array

**Date:** 14/06/2026

**Aim:** To write a C program to perform addition of two matrices.

**Algorithm:**

1. Start
2. Read the number of rows (r) and columns (c)
3. Read elements of first matrix A[][] row by row
4. Read elements of second matrix B[][] row by row
5. Set i = 0, repeat steps 6 to 8 until i reaches r
6. Set j = 0, repeat step 7 until j reaches c
7. Compute C[i][j] = A[i][j] + B[i][j] and increment j
8. Increment i
9. Set i = 0, repeat steps 10 to 12 until i reaches r
10. Set j = 0, repeat step 11 until j reaches c
11. Print C[i][j] and increment j
12. Move to next line and increment i
13. Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>

void main() {
    int a[10][10], b[10][10], c[10][10];
    int r, col, i, j;
    clrscr();
    printf("Enter rows and columns: ");
    scanf("%d %d", &r, &col);
    printf("Enter elements of Matrix A:\n");
    for(i = 0; i < r; i++)
        for(j = 0; j < col; j++)
            scanf("%d", &a[i][j]);
    printf("Enter elements of Matrix B:\n");
    for(i = 0; i < r; i++)
        for(j = 0; j < col; j++)
            scanf("%d", &b[i][j]);
    for(i = 0; i < r; i++)
        for(j = 0; j < col; j++)
            c[i][j] = a[i][j] + b[i][j];
    printf("Resultant Matrix:\n");
    for(i = 0; i < r; i++) {
        for(j = 0; j < col; j++)
            printf("%d ", c[i][j]);
        printf("\n");
    }
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Enter rows and columns: 2 2
Enter elements of Matrix A:
1 2
3 4
Enter elements of Matrix B:
5 6
7 8
Resultant Matrix:
6 8
10 12
```

---

## Experiment 15: Sum of Elements of an Array

**Date:** 14/06/2026

**Aim:** To write a C program to find the sum of all elements in an array.

**Algorithm:**

1. Start
2. Read the number of elements n
3. Read n elements into array arr[]
4. Set sum = 0
5. For i = 0 to n-1, add arr[i] to sum
6. Print sum
7. Stop

**Source Code:**

```c
#include<stdio.h>
#include<conio.h>

void main() {
    int arr[100], n, i, sum = 0;
    clrscr();
    printf("Enter number of elements: ");
    scanf("%d", &n);
    printf("Enter elements: ");
    for(i = 0; i < n; i++)
        scanf("%d", &arr[i]);
    for(i = 0; i < n; i++)
        sum = sum + arr[i];
    printf("Sum of elements: %d", sum);
    getch();
}
```

**Result:** The program was successfully compiled and the output was obtained.

**Output:**

```
Enter number of elements: 5
Enter elements: 10 20 30 40 50
Sum of elements: 150
```