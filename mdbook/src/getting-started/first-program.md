# Your First Program

Now that you have GLaDOS installed, let's write your first program!

## Hello World

Create a file called `hello.c`:

```c
int main() {
    int x = 5;
    int y = 10;
    int result = x + y;
    return result;
}
```

### Compile and Run

```bash
./glados < hello.c
```

**Expected output:**
```
15
```

Congratulations! You've just compiled and run your first GLaDOS program. The program adds two numbers and returns the result.

## Quick Examples

Let's explore a few more examples to get familiar with the language.

### Factorial

This example demonstrates recursion and conditional logic:

```c
int factorial(int n) {
    if (n <= 1) {
        return 1;
    }
    return n * factorial(n - 1);
}

int main() {
    int result = factorial(5);
    return result;
}
```

**Output:** `120`

The factorial function calls itself recursively to calculate 5! = 5 × 4 × 3 × 2 × 1.

### Fibonacci

Another recursive example:

```c
int fib(int n) {
    if (n <= 1) {
        return n;
    }
    return fib(n - 1) + fib(n - 2);
}

int main() {
    return fib(10);
}
```

**Output:** `55`

This calculates the 10th Fibonacci number using recursion.

## Understanding the Basics

### Program Structure

Every GLaDOS program must have a `main` function that returns an integer:

```c
int main() {
    // Your code here
    return 0;
}
```

### Variables

Variables must be declared with a type:

```c
int x = 42;
bool flag = true;
```

### Functions

Functions have a return type, name, parameters, and body:

```c
int add(int a, int b) {
    return a + b;
}
```

## Next Steps

Now that you've written your first programs, you can:

- Explore more [Examples](./examples.md)
- Learn the full [Syntax Guide](../language/syntax.md)
- Understand the [Type System](../language/types.md)
