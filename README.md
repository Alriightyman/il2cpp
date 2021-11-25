il2cpp
===

> 「  While enjoying the efficiency of C# development, obtain the deadly optimized execution speed of the C++ compiler  」

![alt tag](https://github.com/anydream/il2cpp/raw/master/il2cpp-schematic.png)

## How to test
  - Pre-requirements:
    1. Windows 7 or later, 64-bit system;
    2. Visual Studio **2017**, C# and C++ desktop dev environments;
  - Open ``il2cpp.sln``;
  - Set ``test`` as startup project;
  - Run.
  - You can add your test code into ``CodeGenTests.cs`` like this:
    ```CSharp
    [CodeGen]
    static class MyTest
    {
        // return 0 means PASS, otherwise means FAIL
        public static int Entry()
        {
            int a = 1, b = 2;
            if (a + b != 3)
                return 1;
            return 0;
        }
    }
    ```
  - Run ``test`` project to test your code.

## Exchange group
  - ``QQ:548409690``

## Realized features
- [x] Reference analysis of types/methods/fields, extracting the least dependent subset
- [x] Virtual method call and virtual table binding
- [x] Explicit rewriting of interface and base class methods
- [x] Covariance/conversion analysis
- [x] Embedded conservative garbage collector
- [x] Static constructor
- [x] Try/catch/finally/fault exception block analysis and code generation
- [x] Code generation of one-dimensional array/multi-dimensional array
- [x] Enumeration type handling
- [x] String constant code generation
- [x] Nullable type code generation
- [x] Explicit field layout and structure length
- [x] Method delegation
- [x] C++ code compilation tool
- [x] Array read and write instructions
- [x] Stack operation instructions
- [x] Constant load instruction
- [x] Method call instruction
- [x] Variable/parameter/field read and write instructions
- [x] Conditions and branch instructions
- [x] Comparison instruction
- [x] Numerical conversion instruction
- [x] Numerical operation instructions
- [x] Reference and value type object manipulation instructions
- [x] Pointer read and write instructions
- [x] Exception handling instructions
- [x] Boxing/Unboxing Instructions
- [x] Overflow check instruction

## Explicitly unsupported features
- [x] Create a new type at runtime (TypeBuilder.CreateType)
- [x] Generate and execute machine code at runtime (Emit/Expression Trees)
- [x] Load .NET DLL at runtime and instantiate the types in it
- [x] Instantiate generic expansions that do not exist at runtime (only support generic expansions that exist at compile time)
- [x] Add/delete/modify reflection information at runtime
- [x] Recursive expansion of generic parameter types
- [x] Marshaling non-static method delegate


**Under development in full swing...**<br>
**Seeking star, seeking test~**
