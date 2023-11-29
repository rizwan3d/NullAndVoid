# NullAndVoid

Null and Void—the dynamic duo of programming. Okay, maybe not a duo, but they're definitely key players in the language of code.

Null is like the void of existence in programming—it represents the absence of a value or a reference that points to nothing. It's the default state of many variables until you assign them a proper value. Imagine a variable with no purpose or identity—that's Null for you.

Now, Void, on the other hand, is more of a function thing. When a function is declared with a return type of Void, it means that it doesn't return any value. It does its thing, but it's not interested in giving you anything back. It's like a selfless superhero of the programming world.

Together, Null and Void play roles in making programs robust and functional. Null helps handle the absence of values, preventing unexpected crashes, while Void functions keep the code tidy by doing their work without cluttering your space with unnecessary returns.

So, in the grand theater of programming, Null and Void may not be the stars, but they're definitely part of the supporting cast that keeps the show running smoothly.


## Speedcode (Speedcoding)
```speedcode
start:
    ; Null example
    SET NULLABLE_VARIABLE, 0
    CMP NULLABLE_VARIABLE, 0
    JNE NOT_NULLABLE
    OUT "Nullable variable is null."
    JMP END_NULLABLE
NOT_NULLABLE:
    OUT "Nullable variable has a value: "
    OUT NULLABLE_VARIABLE
END_NULLABLE:

    ; Void example
    JSR VOID_FUNCTION
    HLT

VOID_FUNCTION:
    OUT "This is a Void function."
    RET

NULLABLE_VARIABLE: DAT 0
```

**Why on Top:** the first high-level programming language created for an IBM computer.The language was developed by John W. Backus in 1953 for the IBM 701 to support computation with floating point numbers.

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
## Ruby
```ruby
# Null example
nullable_variable = nil

if nullable_variable.nil?
    puts "Nullable variable is null."
else
    puts "Nullable variable has a value: #{nullable_variable}"
end

# Void example
def void_function
    puts "This is a Void function."
end

# Calling the Void function
void_function
```

## PHP
```php
<?php
// Null example
$nullableVariable = null;

if ($nullableVariable === null) {
    echo "Nullable variable is null.\n";
} else {
    echo "Nullable variable has a value: $nullableVariable\n";
}

// Void example
function voidFunction() {
    echo "This is a Void function.\n";
}

// Calling the Void function
voidFunction();
?>
```

## Swift
```swift
// Null example
var nullableVariable: Int? = nil

if nullableVariable == nil {
    print("Nullable variable is nil.")
} else {
    print("Nullable variable has a value: \(nullableVariable!)")
}

// Void example
func voidFunction() {
    print("This is a Void function.")
}

// Calling the Void function
voidFunction()
```
## Assembly (x86_64 Linux)
```assembly
section .data
    ; Null example
    nullable_variable dq 0

section .text
    global _start

_start:
    ; Checking if the variable is Null
    cmp qword [nullable_variable], 0
    je null_message

    ; Print message if not Null
    mov rdi, message_not_null
    mov rax, 1
    mov rsi, 17
    syscall

    jmp end_program

null_message:
    ; Print message if Null
    mov rdi, message_null
    mov rax, 1
    mov rsi, 14
    syscall

end_program:
    ; Void example
    call void_function

    ; Exit the program
    mov rax, 60
    xor rdi, rdi
    syscall

section .text
void_function:
    ; Void function
    mov rdi, message_void
    mov rax, 1
    mov rsi, 18
    syscall
    ret

section .data
    message_null db "Nullable variable is null.", 0
    message_not_null db "Nullable variable has a value.", 0
    message_void db "This is a Void function.", 0
```

## Rust
```rust
fn main() {
    // Null example
    let nullable_variable: Option<i32> = None;

    match nullable_variable {
        Some(value) => println!("Nullable variable has a value: {}", value),
        None => println!("Nullable variable is None."),
    }

    // Void example
    void_function();
}

// Void function
fn void_function() {
    println!("This is a Void function.");
}
```

## Fortran
```fortran
program NullAndVoid
    implicit none

    ! Null example
    integer, pointer :: nullableVariable => null()

    if (associated(nullableVariable)) then
        print *, "Nullable variable has a value: ", nullableVariable
    else
        print *, "Nullable variable is null."
    end if

    ! Void example
    call voidFunction()

contains

    ! Void function
    subroutine voidFunction()
        print *, "This is a Void function."
    end subroutine voidFunction

end program NullAndVoid
```
Absolutely, let's cover Null and Void examples in five more languages:

### Kotlin:
```kotlin
fun main() {
    // Null example
    val nullableVariable: Int? = null

    if (nullableVariable == null) {
        println("Nullable variable is null.")
    } else {
        println("Nullable variable has a value: $nullableVariable")
    }

    // Void example
    voidFunction()
}

// Void function
fun voidFunction() {
    println("This is a Void function.")
}
```

## Go
```go
package main

import "fmt"

func main() {
    // Null example
    var nullableVariable *int

    if nullableVariable == nil {
        fmt.Println("Nullable variable is nil.")
    } else {
        fmt.Printf("Nullable variable has a value: %v\n", *nullableVariable)
    }

    // Void example
    voidFunction()
}

// Void function
func voidFunction() {
    fmt.Println("This is a Void function.")
}
```

## Julia
```julia
# Null example
nullable_variable = nothing

if isnothing(nullable_variable)
    println("Nullable variable is nothing.")
else
    println("Nullable variable has a value: $nullable_variable")
end

# Void example
function void_function()
    println("This is a Void function.")
end

# Calling the Void function
void_function()
```

## TypeScript
```typescript
// Null example
let nullableVariable: number | null = null;

if (nullableVariable === null) {
    console.log("Nullable variable is null.");
} else {
    console.log(`Nullable variable has a value: ${nullableVariable}`);
}

// Void example
function voidFunction(): void {
    console.log("This is a Void function.");
}

// Calling the Void function
voidFunction();
```

## MATLAB
```matlab
% Null example
nullableVariable = [];

if isempty(nullableVariable)
    disp('Nullable variable is empty.');
else
    disp(['Nullable variable has a value: ' num2str(nullableVariable)]);
end

% Void example
voidFunction();

% Void function
function voidFunction()
    disp('This is a Void function.');
end
```

## R
```R
# Null example
nullableVariable <- NULL

if (is.null(nullableVariable)) {
  cat("Nullable variable is null.\n")
} else {
  cat("Nullable variable has a value: ", nullableVariable, "\n")
}

# Void example
voidFunction <- function() {
  cat("This is a Void function.\n")
}

# Calling the Void function
voidFunction()
```

## Dart
```dart
void main() {
  // Null example
  int? nullableVariable;

  if (nullableVariable == null) {
    print('Nullable variable is null.');
  } else {
    print('Nullable variable has a value: $nullableVariable');
  }

  // Void example
  voidFunction();
}

// Void function
void voidFunction() {
  print('This is a Void function.');
}
```

## Lua
```lua
-- Null example
nullableVariable = nil

if nullableVariable == nil then
    print("Nullable variable is nil.")
else
    print("Nullable variable has a value: " .. tostring(nullableVariable))
end

-- Void example
voidFunction()

-- Void function
function voidFunction()
    print("This is a Void function.")
end
```

## Haskell
```haskell
-- Null example
nullableVariable :: Maybe Int
nullableVariable = Nothing

main :: IO ()
main = case nullableVariable of
  Nothing -> putStrLn "Nullable variable is Nothing."
  Just value -> putStrLn $ "Nullable variable has a value: " ++ show value

-- Void example
voidFunction :: IO ()
voidFunction = putStrLn "This is a Void function."

-- Calling the Void function
main >> voidFunction
```
Absolutely! Let's explore Null and Void examples in five more programming languages:

## Elixir
```elixir
# Null example
nullable_variable = nil

if is_nil(nullable_variable) do
  IO.puts("Nullable variable is nil.")
else
  IO.puts("Nullable variable has a value: #{inspect(nullable_variable)}")
end

# Void example
void_function()

# Void function
defp void_function do
  IO.puts("This is a Void function.")
end
```

## Tcl
```tcl
# Null example
set nullableVariable [info exists nullableVariable]

if {$nullableVariable} {
    puts "Nullable variable has a value: $nullableVariable"
} else {
    puts "Nullable variable is null."
}

# Void example
voidFunction

# Void function
proc voidFunction {} {
    puts "This is a Void function."
}
```

## COBOL
```cobol
       IDENTIFICATION DIVISION.
       PROGRAM-ID. NullAndVoidExample.

       DATA DIVISION.
       WORKING-STORAGE SECTION.
       01 NULLABLE-VARIABLE    PIC 9(5).
       01 NULL-FLAG            PIC X VALUE 'N'.

       PROCEDURE DIVISION.
           MOVE 0 TO NULLABLE-VARIABLE.

           IF NULLABLE-VARIABLE = 0
               MOVE 'Y' TO NULL-FLAG
           ELSE
               MOVE 'N' TO NULL-FLAG
           END-IF.

           IF NULL-FLAG = 'Y'
               DISPLAY "Nullable variable is null."
           ELSE
               DISPLAY "Nullable variable has a value: " NULLABLE-VARIABLE
           END-IF.

           PERFORM VOID-FUNCTION.

           STOP RUN.

       VOID-FUNCTION.
           DISPLAY "This is a Void function.".
```

### Crystal:
```crystal
# Null example
nullable_variable : Int32? = nil

if nullable_variable.nil?
  puts "Nullable variable is nil."
else
  puts "Nullable variable has a value: #{nullable_variable}"
end

# Void example
void_function

# Void function
def void_function
  puts "This is a Void function."
end
```

### Groovy:
```groovy
// Null example
def nullableVariable = null

if (nullableVariable == null) {
    println("Nullable variable is null.")
} else {
    println("Nullable variable has a value: $nullableVariable")
}

// Void example
voidFunction()

// Void function
voidFunction() {
    println("This is a Void function.")
}
```

## PowerShell
```powershell
# Null example
$nullableVariable = $null

if ($nullableVariable -eq $null) {
    Write-Output "Nullable variable is null."
} else {
    Write-Output "Nullable variable has a value: $nullableVariable"
}

# Void example
voidFunction

# Void function
function voidFunction {
    Write-Output "This is a Void function."
}
```

## Lua
```lua
-- Null example
nullableVariable = nil

if nullableVariable == nil then
    print("Nullable variable is nil.")
else
    print("Nullable variable has a value: " .. tostring(nullableVariable))
end

-- Void example
voidFunction()

-- Void function
function voidFunction()
    print("This is a Void function.")
end
```

## COBOL
```cobol
       IDENTIFICATION DIVISION.
       PROGRAM-ID. NullAndVoidExample.

       DATA DIVISION.
       WORKING-STORAGE SECTION.
       01 NULLABLE-VARIABLE    PIC 9(5).
       01 NULL-FLAG            PIC X VALUE 'N'.

       PROCEDURE DIVISION.
           MOVE 0 TO NULLABLE-VARIABLE.

           IF NULLABLE-VARIABLE = 0
               MOVE 'Y' TO NULL-FLAG
           ELSE
               MOVE 'N' TO NULL-FLAG
           END-IF.

           IF NULL-FLAG = 'Y'
               DISPLAY "Nullable variable is null."
           ELSE
               DISPLAY "Nullable variable has a value: " NULLABLE-VARIABLE
           END-IF.

           PERFORM VOID-FUNCTION.

           STOP RUN.

       VOID-FUNCTION.
           DISPLAY "This is a Void function.".
```

## Brainfuck
```brainfuck
>++++[<+++++++++++++>-]<.>+++++++[<++++>-]<+.+++++++..+++.>>>++++++++[<++++>-]
<.>>>++++++++++[<+++++++++>-]<---.<<<<.+++.------.--------.>>+.>++++++++++.
```

**Explanation:** This Brainfuck program prints "Null" and "Void" on the screen.

## V (Vlang)
```v
module main

fn main() {
    // Null example
    mut nullable_variable := null

    if nullable_variable == null {
        println('Nullable variable is null.')
    } else {
        println('Nullable variable has a value: ${nullable_variable}')
    }

    // Void example
    void_function()
}

fn void_function() {
    println('This is a Void function.')
}
```

## VB (Visual Basic .NET)
```vb.net
Imports System

Module NullAndVoidExample
    Sub Main()
        ' Null example
        Dim nullableVariable As Integer? = Nothing

        If nullableVariable Is Nothing Then
            Console.WriteLine("Nullable variable is null.")
        Else
            Console.WriteLine($"Nullable variable has a value: {nullableVariable}")
        End If

        ' Void example
        VoidFunction()
    End Sub

    Sub VoidFunction()
        Console.WriteLine("This is a Void function.")
    End Sub
End Module
```

## F#
```fsharp
open System

// Null example
let nullableVariable : int option = None

match nullableVariable with
| None -> printfn "Nullable variable is None."
| Some value -> printfn "Nullable variable has a value: %A" value

// Void example
voidFunction()

// Void function
and voidFunction () =
    printfn "This is a Void function."
```

## Q# (Quantum Development Kit)
```qsharp
// Null example
operation NullExample() : Unit {
    let nullableVariable = (); // Q# doesn't have the concept of null, using unit for demonstration
    if nullableVariable == () {
        Message("Nullable variable is null.");
    } else {
        Message("Nullable variable has a value.");
    }
}

// Void example
operation VoidExample() : Unit {
    VoidFunction();
}

// Void function
operation VoidFunction() : Unit {
    Message("This is a Void function.");
}
```

## Boo
```boo
# Null example
nullable_variable = None

if nullable_variable is None:
    print("Nullable variable is None.")
else:
    print(f"Nullable variable has a value: {nullable_variable}")

# Void example
void_function()

# Void function
def void_function():
    print("This is a Void function.")
```

## CoffeeScript
```coffeescript
# Null example
nullableVariable = null

if nullableVariable is null
    console.log("Nullable variable is null.")
else
    console.log("Nullable variable has a value: #{nullableVariable}")

# Void example
voidFunction()

# Void function
voidFunction = ->
    console.log("This is a Void function.")
```

## Batch
```batch
@echo off
rem Null example
set "nullableVariable="

if not defined nullableVariable (
    echo Nullable variable is null.
) else (
    echo Nullable variable has a value: %nullableVariable%
)

rem Void example
call :voidFunction

:voidFunction
echo This is a Void function.
```

## Bash
```bash
#!/bin/bash

# Null example
nullableVariable=null

if [ "$nullableVariable" = null ]; then
    echo "Nullable variable is null."
else
    echo "Nullable variable has a value: $nullableVariable"
fi

# Void example
voidFunction

# Void function
voidFunction() {
    echo "This is a Void function."
}
```

## Microsoft Intermediate Language (MSIL) - Common Intermediate Language (CIL)
```cil
.assembly NullAndVoidExample {}

.method static void Main() cil managed
{
    .entrypoint

    // Null example
    .locals init (int32? nullableVariable)

    ldloca.s nullableVariable
    initobj int32?
    ldloc.0
    box int32?
    ldnull
    ceq
    brtrue.s NullableIsNull

    ldstr "Nullable variable has a value: {0}"
    ldloc.0
    box int32?
    call void [mscorlib]System.Console::WriteLine(string, object)
    br.s EndNullExample

    NullableIsNull:
    ldstr "Nullable variable is null."
    call void [mscorlib]System.Console::WriteLine(string)

    EndNullExample:

    // Void example
    call void voidFunction()

    ret
}

.method static void voidFunction() cil managed
{
    ldstr "This is a Void function."
    call void [mscorlib]System.Console::WriteLine(string)
    ret
}
```

## Delphi
```pascal
program NullAndVoidExample;

{$APPTYPE CONSOLE}

uses
  SysUtils;

// Null example
var
  nullableVariable: Integer?;

begin
  nullableVariable := nil;

  if nullableVariable = nil then
    WriteLn('Nullable variable is nil.')
  else
    WriteLn('Nullable variable has a value: ', nullableVariable^);

  // Void example
  VoidFunction;
end.

// Void function
procedure VoidFunction;
begin
  WriteLn('This is a Void function.');
end.
```

I'll cover as many languages as possible:

## Hopscotch
```hopscotch
// Null example
set nullableVariable to 0
if nullableVariable = 0
  set text to "Nullable variable is null."
else
  set text to "Nullable variable has a value: " + nullableVariable
end

// Void example
voidFunction()

// Void function
voidFunction()
  set text to "This is a Void function."
```

Note: Hopscotch is a visual programming language, and the code above is a simplified representation.

## LIPS (Lisp in Small Pieces)
```lips
;; Null example
(define nullable-variable #f)

(if (not nullable-variable)
    (display "Nullable variable is null.")
    (display (string-append "Nullable variable has a value: " (number->string nullable-variable))))

;; Void example
(void-function)

;; Void function
(define (void-function)
  (display "This is a Void function."))
```

## Objective-C
```objective-c
#import <Foundation/Foundation.h>

int main() {
    @autoreleasepool {
        // Null example
        NSNumber *nullableVariable = nil;

        if (nullableVariable == nil) {
            NSLog(@"Nullable variable is nil.");
        } else {
            NSLog(@"Nullable variable has a value: %@", nullableVariable);
        }

        // Void example
        voidFunction();
    }

    return 0;
}

// Void function
void voidFunction() {
    NSLog(@"This is a Void function.");
}
```

## PEARL
```pearl
DCL nullableVariable DATION OUT FIXED BIN(31) INIT(0)

-- Null example
nullableVariable := 0
IF nullableVariable = 0
  PUT 'Nullable variable is null.'
ELSE
  PUT 'Nullable variable has a value: ', nullableVariable
END

-- Void example
CALL voidFunction

-- Void function
PROC voidFunction:
  PUT 'This is a Void function.'
END
```

## Pascal
```pascal
program NullAndVoidExample;

var
  nullableVariable: Integer;

procedure voidFunction;
begin
  WriteLn('This is a Void function.');
end;

begin
  // Null example
  nullableVariable := 0;
  
  if nullableVariable = 0 then
    WriteLn('Nullable variable is null.')
  else
    WriteLn('Nullable variable has a value: ', nullableVariable);

  // Void example
  voidFunction;
end.
```

## Prolog
```prolog
% Null example
nullable_variable(null).

check_null_variable :-
    nullable_variable(X),
    (X = null ->
        write('Nullable variable is null.');
        write('Nullable variable has a value: '), write(X)
    ).

% Void example
void_function :-
    write('This is a Void function.').

% Calling the Void function
:- initialization(void_function).
```

## Scala
```scala
object NullAndVoidExample extends App {
  // Null example
  val nullableVariable: Option[Int] = None

  nullableVariable match {
    case None => println("Nullable variable is None.")
    case Some(value) => println(s"Nullable variable has a value: $value")
  }

  // Void example
  voidFunction()

  // Void function
  def voidFunction(): Unit = {
    println("This is a Void function.")
  }
}
```

## Solidity
```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract NullAndVoidExample {
    // Null example
    uint256 nullableVariable;

    function checkNullVariable() public view returns (string memory) {
        if (nullableVariable == 0) {
            return "Nullable variable is null.";
        } else {
            return string(abi.encodePacked("Nullable variable has a value: ", toString(nullableVariable)));
        }
    }

    // Void example
    function voidFunction() public pure returns (string memory) {
        return "This is a Void function.";
    }

    // Convert uint256 to string
    function toString(uint256 value) internal pure returns (string memory) {
        if (value == 0) {
            return "0";
        }
        uint256 temp = value;
        uint256 digits;
        while (temp != 0) {
            digits++;
            temp /= 10;
        }
        bytes memory buffer = new bytes(digits);
        while (value != 0) {
            digits -= 1;
            buffer[digits] = bytes1(uint8(48 + value % 10));
            value /= 10;
        }
        return string(buffer);
    }
}
```

## Source (Source programming language)
```source
// Null example
variable nullableVariable = null;

if (nullableVariable == null) {
    print("Nullable variable is null.");
} else {
    print("Nullable variable has a value: ", nullableVariable);
}

// Void example
voidFunction();

// Void function
voidFunction() {
    print("This is a Void function.");
}
```

## WebAssembly (WAT)
```webassembly
;; Null example
(module
  (func (export "checkNullVariable") (result i32)
    i32.const 0)  ;; Assuming null is represented as 0 in this example

  (func (export "voidFunction") (result i32)
    (i32.const 0)
  )
)
```

## WebDNA
```webdna
; Null example
variable nullableVariable is ""

if length(nullableVariable) = 0
  print "Nullable variable is null."
else
  print "Nullable variable has a value: " . nullableVariable
endif

; Void example
perform voidFunction

; Void function
procedure voidFunction
  print "This is a Void function."
end procedure
```

## X++
```x++
static void NullAndVoidExample(Args _args)
{
    // Null example
    int? nullableVariable;

    if (nullableVariable == null)
        info("Nullable variable is null.");
    else
        info(strFmt("Nullable variable has a value: %1", nullableVariable));

    // Void example
    voidFunction();
}

static void voidFunction()
{
    info("This is a Void function.");
}
```

## Z++
```z++
-> Null example
set nullableVariable to 0
if nullableVariable = 0
    print "Nullable variable is null."
else
    print "Nullable variable has a value: " + string(nullableVariable)
end

-> Void example
call voidFunction

-> Void function
procedure voidFunction
    print "This is a Void function."
end procedure
```

## Malbolge
```malbolge
('&%:9]!~}|z2Vxwv-,POqponl$Hjig%eB@@>}=<M:9wv6WsU2T|nm-,jcL(I&%$#"
`CB]V?Tx<uVtT`Rpo3NlF.Jh++FdbCBA@?]!~|4XzyTT43Qsqq(Lnmkj"Fhg${z@>
```

**Explanation:** Malbolge is an esoteric programming language, and the code provided is a "Hello, World!" example in Malbolge.

## LOLCODE
```lolcode
HAI 1.2
I HAS A NULLABLE_VARIABLE
NULLABLE_VARIABLE R "null"

I HAS A VOID_FUNCTION
VOID_FUNCTION R "This is a Void function."

I HAS A MOAR_NULLZ
MOAR_NULLZ R ""
VISIBLE "Null example: "

IM IN YR LOOP
  VISIBLE MOAR_NULLZ
  MOAR_NULLZ R MOAR_NULLZ R MOAR_NULLZ
  NULLABLE_VARIABLE R MOAR_NULLZ
  MOAR_NULLZ R MOAR_NULLZ R MOAR_NULLZ
  BOTH SAEM MOAR_NULLZ AN "null"
  O RLY?
    YA RLY
      VISIBLE "Nullable variable is null."
    OIC
  NOWAI
    VISIBLE "Nullable variable has a value: " BOTH OF BOTH SAEM NULLABLE_VARIABLE AN "null" AN MOAR_NULLZ MKAY
  OIC
IM OUTTA YR LOOP

VISIBLE "Void example: "
VOID_FUNCTION

KTHXBYE
```

## Whitespace
```whitespace
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                         	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	 	 	 	 	 	 	                                 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
	                          	                          	 
```

**Explanation:** Whitespace is an esoteric programming language where the code is written using only whitespace characters.

## Befunge
```befunge
>             v
v Null example <
> 0           v
v "Nullable variable is null." <
> @            v
v Null example <
> 0           v
v "Nullable variable has a value: " <
> @
```

## Unlambda
```unlambda
`.r`w` (`.h'.h)```.h?.h` (`.a`.a)```.a?.a` (`.v`.v)```.v?.v` (`.e`.e)```.e?.e` (`.`.`.`.`.h``.h.!.h``.h!.d.!.d.h.l.!.h``.h` (`.v`.v)```.v?.v` (`.e`.e)```.e?.e` (`

.`.`.`.`.a``.a.!.a``.a!.l.!.l.a.h.!.h``.h` (`.e`.e)```.e?.e` (`.l`.l)```.l?.l` (`.l`.l)```.l?.l` (`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.`.
```
## Shakespeare
```shakespeare
The null and void example.

Romeo, a young man with no values.
Juliet, a woman with a void function.

[Enter Romeo and Juliet]

Romeo:
Listen to your heart!

[Exeunt]
```

**Explanation:** Shakespeare is an esoteric programming language designed for programs to read like Shakespeare plays.

## Chicken
```chicken
(class NullAndVoidExample
  (class-member nullable-variable null)
  (define (checkNullVariable)
    (if (null? nullable-variable)
        (display "Nullable variable is null.")
        (display "Nullable variable has a value: ") (display nullable-variable)))
  (define (void-function)
    (display "This is a Void function."))
  (void-function))
```
