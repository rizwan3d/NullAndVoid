# NullAndVoid

Null and Void—the dynamic duo of programming. Okay, maybe not a duo, but they're definitely key players in the language of code.

Null is like the void of existence in programming—it represents the absence of a value or a reference that points to nothing. It's the default state of many variables until you assign them a proper value. Imagine a variable with no purpose or identity—that's Null for you.

Now, Void, on the other hand, is more of a function thing. When a function is declared with a return type of Void, it means that it doesn't return any value. It does its thing, but it's not interested in giving you anything back. It's like a selfless superhero of the programming world.

Together, Null and Void play roles in making programs robust and functional. Null helps handle the absence of values, preventing unexpected crashes, while Void functions keep the code tidy by doing their work without cluttering your space with unnecessary returns.

So, in the grand theater of programming, Null and Void may not be the stars, but they're definitely part of the supporting cast that keeps the show running smoothly.

## Pyhton
```py
def null_example():
    # Initializing a variable with Null
    null_variable = None

    # Checking if the variable is Null
    if null_variable is None:
        print("This variable is Null.")
    else:
        print("This variable is not Null.")

def void_example():
    # A Void function that prints a message without returning anything
    def print_message():
        print("This is a Void function.")

    # Calling the Void function
    print_message()

# Let's play with Null and Void!
null_example()
void_example()
```

## C#
```c#
using System;

class NullAndVoidExample
{
    static void Main()
    {
        // Null example
        int? nullableInt = null;

        if (nullableInt.HasValue)
        {
            Console.WriteLine($"Nullable int value: {nullableInt.Value}");
        }
        else
        {
            Console.WriteLine("Nullable int is null.");
        }

        // Void example
        void voidFunction()
        {
            Console.WriteLine("This is a Void function.");
        }

        // Calling the Void function
        voidFunction();
    }
}
```

## JavaScript
```js
// Null example
let nullableVariable = null;

if (nullableVariable === null) {
    console.log("Nullable variable is null.");
} else {
    console.log(`Nullable variable has a value: ${nullableVariable}`);
}

// Void example
function voidFunction() {
    console.log("This is a Void function.");
}

// Calling the Void function
voidFunction();
```

## C++
```c++
#include <iostream>

// Null example
int main() {
    // Null pointer
    int* nullablePointer = nullptr;

    if (nullablePointer == nullptr) {
        std::cout << "Nullable pointer is null." << std::endl;
    } else {
        std::cout << "Nullable pointer has a value." << std::endl;
    }

    // Void example
    void voidFunction() {
        std::cout << "This is a Void function." << std::endl;
    }

    // Calling the Void function
    voidFunction();

    return 0;
}
```

## C
```c
#include <stdio.h>

// Null example
int main() {
    // Null pointer
    int *nullablePointer = NULL;

    if (nullablePointer == NULL) {
        printf("Nullable pointer is null.\n");
    } else {
        printf("Nullable pointer has a value.\n");
    }

    // Void example
    void voidFunction() {
        printf("This is a Void function.\n");
    }

    // Calling the Void function
    voidFunction();

    return 0;
}
```

## Java
```java
public class NullAndVoidExample {
    public static void main(String[] args) {
        // Null example
        Integer nullableInteger = null;

        if (nullableInteger == null) {
            System.out.println("Nullable integer is null.");
        } else {
            System.out.println("Nullable integer has a value: " + nullableInteger);
        }

        // Void example
        voidFunction();
    }

    // Void function
    private static void voidFunction() {
        System.out.println("This is a Void function.");
    }
}
```
