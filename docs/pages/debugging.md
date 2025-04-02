# Debugging in VS Code
In this section, we will talk about how to debug your Python code using VS Code. 
You'll use features like **Step Into**, **Step Over,** and **Step Out**. These tools help you see what happens inside your functions and loops. We’ll use a simple program that adds and multiplies numbers.

## Create Your Python File
1. Open VS Code.
2. Open a folder where you want to work.
3. Create a new file and name it `simple_debug.py`.

<figure markdown="span">
  ![Image title](../assets/debug1.png){ width="100%" }
</figure>


## Enter the Code

Copy and paste the following code into your `simple_debug.py` file:

``` { .py }
def add(a, b):
    sum = a + b
    return sum

def multiply(x, y):
    result = 0
    for i in range(y):
        result = add(result, x)
    return result

def main():
    num1 = 4
    num2 = 3
    product = multiply(num1, num2)
    print("Product is:", product)

main()
```
This code defines two functions: `add` (which adds two numbers) and `multiply` (which uses repeated addition to multiply two numbers). The `main` function calls `multiply` and prints the result.

## Open the Debug panel

1. Click the Run and Debug icon (the bug icon) on the left sidebar.
2. Alternatively, press `Ctrl` + `Shift` + `D` 

<figure markdown="span">
  ![Image title](../assets/debug3.png){ width="100%" }
</figure>


## Set Breakpoints
Breakpoints allow you to pause your program at specific lines to see what is happening.

1. Move your mouse over the left side of the line numbers.
2. You'll notice a dim red dot appear. Click on it, and it will turn into a solid red dot, indicating that a breakpoint has been set.

Set breakpoints at:

1. The line `result = add(result, x)` inside the `multiply()` function (to see when the `add()` function is called).

<figure markdown="span">
  ![Image title](../assets/debug4.gif){ width="100%" }
</figure>


## Start Debugging
1. Click the `Run and Debug` button at the top of the Debug panel.
2. Your code will run and pause at the breakpoint.

<figure markdown="span">
  ![Image title](../assets/debug5.gif){ width="100%" }
</figure>


## Where to Inspect Variables
1. **Variables section**: When the code pauses at a breakpoint, you can see the current values of your variables in the **Variables** section on the left side of the Debug panel. 
2. **Inline code**: You can also see the current values for variables (like `i` and `y`) displayed inline in the code, making it easy to track them as you step through.

<figure markdown="span">
  ![Image title](../assets/debug6.png){ width="100%" }
</figure>


## Step Into: See Inside a Function
1. When you reach the line `result = add(result, x)` in the `multiply()` function, click the **Step Into** button (down arrow icon).
2. VS Code will take you inside the `add()` function.
3. Now you can see how the values `a` and `b` are added together.

<figure markdown="span">
  ![Image title](../assets/debug7.gif){ width="100%" }
</figure>

Tip: Use this to understand how each function works.


## Step Out: Exit the Current Function
1. If you are inside a function (like `add()`) and want to return to the function that called it, click the **Step Out** button (up arrow icon).
2. This will finish the current function and take you back to the previous level in your code.

<figure markdown="span">
  ![Image title](../assets/debug8.gif){ width="100%" }
</figure>

## Step Over: Skip the Function Details
1. If you don’t want to see inside the `add()` function, you can click the **Step Over** button (curved arrow icon).
2. This will execute the `add()` function but not show its inner workings.
3. Use this to move through your code quickly when you don’t need to see every detail.

<figure markdown="span">
  ![Image title](../assets/debug9.gif){ width="100%" }
</figure>

## Finish Debugging
1. When you’re done, click the red square (stop button) to stop debugging.
2. Check your terminal to see the output (it should display "Product is: 12").

<figure markdown="span">
  ![Image title](../assets/debug10.gif){ width="100%" }
</figure>
