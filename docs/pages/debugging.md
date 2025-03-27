# Debugging Bubble Sort in VS Code
In this section, we will talk about Debugging. This guide clearly shows how to debug a Bubble Sort algorithm in Python using VS Code. It helps you understand the Bubble Sort algorithm and VS Code debugging features step-by-step.

In this section, you'll learn Bubble Sort and VS Code debugging at the same time. You'll see how breakpoints, Step Into, Step Over, and Step Out commands help you understand exactly how Bubble Sort works.

## 1, Create Your Python File
Open VS Code and create a new file named bubble_sort.py

## 2. Enter the Bubble Sort Code
Type or copy the following Python code into your file:
``` { .py }
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(0, n-i-1):
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]

numbers = [64, 34, 25, 12, 22, 11, 90]
bubble_sort(numbers)
print(numbers) 
```

## 3. Activate Debugging
Click the "Run and Debug" icon (bug icon) in the VS Code sidebar.

## 4. Set Breakpoints

``` { .py .annotate }
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):  (1)
        for j in range(0, n-i-1):  (2)
            if arr[j] > arr[j+1]:  (3)
                arr[j], arr[j+1] = arr[j+1], arr[j]

numbers = [64, 34, 25, 12, 22, 11, 90]
bubble_sort(numbers)
print(numbers) 
```

1. Line `4` (outer loop)
2. Line `5` (inner loop)
3. Line `6` (swap operation)

Click next to line numbers to set breakpoints:

- Line `4` (outer loop)
- Line `5` (inner loop)
- Line `6` (swap operation)

## 5. Start Debugging
Press F5 or click the green play button to start debugging.

## 6. Inspect Variables
Hover your mouse over variables like `arr`, `i`, and `j` to view their values.

## 7: Step Through Outer Loop
Press F10 repeatedly to move through each iteration of the outer loop and see the largest elements "bubble" up to their sorted position.

## 8: Step Through Inner Loop
Observe closely how elements are compared:
- Hover over `arr[j]` and `arr[j+1]`.
- Press F10 to move step-by-step within the inner loop.

## 9: Watch Swapping Elements
When stopped at line 6, carefully check how two elements are swapped:
- Confirm that the larger element moves right.
- Press F10 to execute swaps and observe array changes.

## 10: Complete and Review
- Continue stepping through until sorting is complete.
- Press the red square to stop debugging.
- Check the terminal output to verify the sorted array.

You've successfully debugged and understood Bubble Sort using VS Code!