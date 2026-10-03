# Data Structures Lab – Programs

## Section A: Array Operations

### 1. Insertion in Array

```c
for(i = n; i >= pos; i--)
{
    arr[i] = arr[i - 1];
}
arr[pos - 1] = item;
n++;
```

### 2. Deletion in Array

```c
item = arr[pos - 1];
for(i = pos - 1; i < n - 1; i++)
{
    arr[i] = arr[i + 1];
}
n--;
```

### 3. Sum of Array Elements

```c
sum = 0;
for(i = 0; i < n; i++)
{
    sum = sum + arr[i];
}
```

### 4. Matrix Addition

```c
for(i = 0; i < r; i++)
{
    for(j = 0; j < c; j++)
    {
        c[i][j] = a[i][j] + b[i][j];
    }
}
```

## Section B: Searching

### 5. Linear Search

```c
for(i = 0; i < n; i++)
{
    if(arr[i] == key)
    {
        printf("Found at position %d", i + 1);
        break;
    }
}
```

### 6. Binary Search

```c
low = 0;
high = n - 1;
while(low <= high)
{
    mid = (low + high) / 2;
    if(arr[mid] == key)
    {
        printf("Found");
        break;
    }
    else if(key < arr[mid])
    {
        high = mid - 1;
    }
    else
    {
        low = mid + 1;
    }
}
```

## Section C: Sorting

### 7. Bubble Sort

```c
for(i = 0; i < n - 1; i++)
{
    for(j = 0; j < n - i - 1; j++)
    {
        if(arr[j] > arr[j + 1])
        {
            temp = arr[j];
            arr[j] = arr[j + 1];
            arr[j + 1] = temp;
        }
    }
}
```

### 8. Selection Sort

```c
for(i = 0; i < n - 1; i++)
{
    min = i;
    for(j = i + 1; j < n; j++)
    {
        if(arr[j] < arr[min])
        {
            min = j;
        }
    }
    temp = arr[i];
    arr[i] = arr[min];
    arr[min] = temp;
}
```

### 9. Insertion Sort

```c
for(i = 1; i < n; i++)
{
    key = arr[i];
    j = i - 1;
    while(j >= 0 && arr[j] > key)
    {
        arr[j + 1] = arr[j];
        j--;
    }
    arr[j + 1] = key;
}
```

## Section D: Stack Using Array

### 10. Push

```c
if(top == MAX - 1)
{
    printf("Stack Overflow");
}
else
{
    top++;
    stack[top] = item;
}
```

### Pop

```c
if(top == -1)
{
    printf("Stack Underflow");
}
else
{
    item = stack[top];
    top--;
}
```

### Display

```c
for(i = top; i >= 0; i--)
{
    printf("%d ", stack[i]);
}
```

## Section E: Queue Using Array

### 11. Enqueue

```c
if(rear == MAX - 1)
{
    printf("Queue Overflow");
}
else
{
    if(front == -1)
    {
        front = 0;
    }
    rear++;
    queue[rear] = item;
}
```

### Dequeue

```c
if(front == -1 || front > rear)
{
    printf("Queue Underflow");
}
else
{
    item = queue[front];
    front++;
}
```

### Display

```c
for(i = front; i <= rear; i++)
{
    printf("%d ", queue[i]);
}
```