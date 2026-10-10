
## Installation & Setup

Before writing code, you need to set up your computer. Pick your operating system below and follow the steps in order.

🍎 macOS🪟 Windows

1. 1
    
    **Install Visual Studio Code**The code editor where you'll write your programs.
    
2. 2
    
    **Install Xcode Command Line Tools**This gives you the C++ compiler on Mac.xcode-select--install
    
3. 3
    
    **Install the C/C++ Extension in VS Code**Search "C/C++" in the Extensions tab and install it.
    
4. 4
    
    **Verify the compiler is installed**Run this in the terminal — a version number means success.clang++--version
    
5. 5
    
    **Create, compile, and run your first program**You're ready to write code! (See section 3.)
    

02

## Boiler Plate

Every C++ program starts with the same basic code. This starter code is called boilerplate.

📌 Definition

Boilerplate is the standard starting code that every C++ program needs before you add your own logic.

**Simple meaning:** The ready-made skeleton you type first, every single time.

main.cpp

```
#include <iostream>
using namespace std;

int main() {
    // write your code here
    return 0;
}
```

`#include <iostream>`Brings in input/output features

`using namespace std;`Lets you write `cout`, not `std::cout`

`int main() { }`Where the program starts running

`return 0;`Tells the system it ran successfully

Key points

- Every program must have a **main()** function.
- Your code goes **inside** the curly braces { }.
- Each statement ends with a semicolon **;**

03

## Write Your First Program

Let's make the program actually do something — print a message on the screen.

hello.cpp

```
#include <iostream>
using namespace std;

int main() {
    cout << "Hello, World!";
    return 0;
}
```

OutputHello, World!

What each part does

- **cout** prints text on the screen.
- Text goes inside **double quotes** " ".
- **<<** sends the text into cout.

MODULE 02

# Fundamentals

The building blocks of every C++ program — variables, types, operators, and how to talk to the user.

01

## Variables & Data Types

Before writing real logic, you need to know how C++ stores and labels data.

### Comments

📌 Definition

A comment is a note written inside your code that the compiler completely ignores.

**Simple meaning:** A message for humans, not for the computer.

comments.cpp

```
// single-line comment

/* multi-line
   comment */
```

- Single-line: **//**
- Multi-line: **/* ... */**
- Used to explain code — never affects the output.

### Syntax

📌 Definition

Syntax is the set of rules that decide how C++ code must be written.

**Simple meaning:** Grammar rules for code — break them, and the compiler throws an error.

- Every statement ends with a semicolon **;**
- Code blocks are wrapped in **{ }**
- C++ is **case-sensitive** — `Age` and `age` are different.

### Word vs Keyword

|Basis|Word|Keyword|
|---|---|---|
|Meaning|Any name you choose|A reserved word in C++|
|Can rename?|Yes|No|
|Example|`age`, `total`|`int`, `return`, `if`|

### Variables

📌 Definition

A variable is a named memory location used to store data that can change during program execution.

**Simple meaning:** A labeled box that holds a value.

variable.cpp

```
int age = 20;
```

- Must be **declared** with a data type before use.
- Its value can **change** later in the program.
- Every variable needs a unique **name**.

### Naming Convention, Identifiers & Literals

Naming rules

- Can contain letters, digits, and underscore **_**
- Cannot start with a digit.
- Cannot use a keyword as a name.
- No spaces allowed.

|Literal Type|Example|
|---|---|
|Integer|`10`, `-5`|
|Floating-point|`3.14`|
|Character|`'A'`|
|String|`"Hello"`|
|Boolean|`true`, `false`|

A literal is a fixed value written directly in code.

### Constants

📌 Definition

A constant is a value that cannot be changed once it is defined.

**Simple meaning:** A locked box — set once, never modified.

constant.cpp

```
const int maxScore = 100;
```

### Data Types

📌 Definition

A data type tells the compiler what kind of value a variable will store.

**Simple meaning:** The "category" of the box's contents — numbers, text, or true/false.

|Type|Stores|Example|
|---|---|---|
|int|Whole numbers|`10`, `-3`|
|float|Decimal numbers|`3.14`|
|double|Larger decimal numbers|`3.14159265`|
|char|A single character|`'A'`|
|bool|true / false|`true`|
|void|No value at all|used for functions|

### Garbage Value

- Happens when you skip giving a variable a starting value.
- The value is leftover data from memory — not zero, not predictable.
- Always initialize variables to avoid this.

### sizeof Operator

📌 Definition

The `sizeof` operator returns the memory size (in bytes) that a data type or variable occupies.

**Simple meaning:** Asks the compiler, "how much space does this take?"

sizeof.cpp

```
cout << sizeof(int);
```

Output4

02

## Type Conversion

Sometimes C++ needs to convert one data type into another. This can happen automatically or manually.

### Implicit Conversion

📌 Definition

Implicit conversion happens automatically when the compiler converts one data type into another without being asked.

**Simple meaning:** The compiler quietly does the conversion for you.

implicit.cpp

```
int a = 5;
double b = a; // int auto-converted to double
```

### Explicit Conversion

📌 Definition

Explicit conversion is when the programmer manually converts a value from one type to another.

**Simple meaning:** You tell the compiler exactly what type to convert to.

explicit.cpp

```
double x = 9.7;
int y = (int)x; // manually converted
```

### Type Casting

📌 Definition

Type casting is the technique used to perform explicit conversion using cast syntax.

**Simple meaning:** The actual "tool" used to force a type change.

- C-style: `(int)x`
- C++-style: `static_cast<int>(x)`

|Basis|Implicit|Explicit|
|---|---|---|
|Done by|Compiler|Programmer|
|Control|Automatic|Manual|
|Risk|May lose data silently|Intentional, controlled|

03

## Operators

Operators let you perform actions on variables and values — math, comparisons, and logic.

### Unary vs Binary

|Basis|Unary|Binary|
|---|---|---|
|Operands needed|1|2|
|Example|`-a`, `++a`|`a + b`|

### Arithmetic Operators

|Operator|Meaning|Example|
|---|---|---|
|`+`|Addition|`a + b`|
|`-`|Subtraction|`a - b`|
|`*`|Multiplication|`a * b`|
|`/`|Division|`a / b`|
|`%`|Modulus (remainder)|`a % b`|

### Relational Operators

|Operator|Meaning|
|---|---|
|`==`|Equal to|
|`!=`|Not equal to|
|`>`|Greater than|
|`<`|Less than|
|`>=`|Greater than or equal to|
|`<=`|Less than or equal to|

### Assignment Operators

|Operator|Meaning|Same as|
|---|---|---|
|`=`|Assign|—|
|`+=`|Add and assign|`a = a + b`|
|`-=`|Subtract and assign|`a = a - b`|
|`*=`|Multiply and assign|`a = a * b`|
|`/=`|Divide and assign|`a = a / b`|
|`%=`|Modulus and assign|`a = a % b`|

### Logical Operators

|Operator|Meaning|Example|
|---|---|---|
|`&&`|AND — true if both are true|`a && b`|
|`\|`|OR — true if either is true|`a \| b`|
|`!`|NOT — reverses the result|`!a`|

04

## Input & Output

How your program talks to the user — taking input and printing output.

### cin

📌 Definition

`cin` is used to take input from the user through the keyboard.

**Simple meaning:** "Console in" — reads what the user types.

cin.cpp

```
int age;
cin >> age;
```

### cout

📌 Definition

`cout` is used to print output to the screen.

**Simple meaning:** "Console out" — displays a value or message.

cout.cpp

```
cout << "Age: " << age;
```

### getline() & cin.ignore()

📌 Definition

`getline()` reads an entire line of text, including spaces — something `cin` alone cannot do.

**Simple meaning:** Use it when the input has more than one word, like a full name.

getline.cpp

```
string fullName;
getline(cin, fullName);
```

### Reading a String After an Int

📌 Definition

When you read a number with `cin` and then a full line with `getline()`, the leftover newline from the number is picked up by `getline()` — so it reads an empty line instead of the real input.

**Simple meaning:** Put `cin.ignore()` between them to throw away that leftover newline.

read-string-after-int.cpp

```
int age;
string name;

cin >> age;          // leftover '\n' stays in the input buffer
cin.ignore();       // throw away that leftover newline
getline(cin, name); // now reads the whole line correctly
```

Skip `cin.ignore()` and `name` comes out empty — a classic beginner bug.

### endl vs \n

|Basis|endl|\n|
|---|---|---|
|What it does|New line + flushes buffer|Just a new line|
|Speed|Slower|Faster|
|Usage|`cout << endl;`|`cout << "\n";`|

### Escape Sequences

|Sequence|Meaning|
|---|---|
|`\n`|New line|
|`\t`|Tab space|
|`\\`|Backslash|
|`\"`|Double quote|
|`\'`|Single quote|

MODULE 03

# Control-Flow Statements

Teach your program to make decisions and repeat actions — conditionals, loops, and jump statements.

01

## Decision Making | Conditional Statements          *(Same as if                                                                                                 else elif ladder)

Conditional statements let your program make choices and run different code based on conditions.

### if

📌 Definition

The `if` statement runs a block of code only when a condition is true.

**Simple meaning:** "If this is true, do this."

if.cpp

```
if (age >= 18) {
    cout << "Adult";
}
```

### if else

📌 Definition

The `if-else` statement runs one block if the condition is true, and a different block if it's false.

**Simple meaning:** "If this, do A — otherwise, do B."

if-else.cpp

```
if (age >= 18) {
    cout << "Adult";
} else {
    cout << "Minor";
}
```

### Nested if

📌 Definition

A nested if is an `if` statement placed inside another `if` statement.

**Simple meaning:** A condition checked only after another condition is already true.

nested-if.cpp

```
if (age >= 18) {
    if (hasID) {
        cout << "Entry allowed";
    }
}
```

### else if Ladder

📌 Definition

An else-if ladder checks multiple conditions one after another, running the block for the first true condition.

**Simple meaning:** A chain of "otherwise, check this next" checks.

else-if.cpp

```
if (marks >= 90) {
    cout << "Grade A";
} else if (marks >= 75) {
    cout << "Grade B";
} else {
    cout << "Grade C";
}
```

### switch case

📌 Definition

The `switch` statement compares one variable against several fixed values, running the matching case.

**Simple meaning:** A cleaner alternative to a long else-if ladder when checking a single value.

switch.cpp

```
switch (day) {
    case 1: cout << "Monday"; break;
    case 2: cout << "Tuesday"; break;
    default: cout << "Invalid";
}
```

- Every `case` should end with a **break**, or execution "falls through" to the next case.
- `default` runs when no case matches.

### Ternary Operator

📌 Definition

The ternary operator is a one-line shortcut for a simple if-else statement.

**Simple meaning:** Squeezes an if-else into a single expression.

ternary.cpp

```
string result = (age >= 18) ? "Adult" : "Minor";
```

Syntax: `condition ? valueIfTrue : valueIfFalse`

### if vs switch

|Basis|if-else Ladder|switch|
|---|---|---|
|Condition type|Ranges & complex conditions|Exact value matches|
|Readability|Harder with many checks|Cleaner for many fixed values|
|Speed|Checks sequentially|Often faster (jump table)|

02

## Loops

Loops let you repeat a block of code multiple times without writing it again and again.

### Why Loops?

- Avoids repeating the same code manually.
- Automates repetitive tasks — printing, counting, calculating.
- Makes programs shorter and easier to maintain.

### Types of Loops

|Loop|Best Used When|
|---|---|
|for|Number of iterations is known|
|while|Number of iterations is unknown|
|do-while|Code must run at least once|

### for Loop

📌 Definition

A `for` loop repeats a block of code a specific number of times.

**Simple meaning:** Best when you already know how many times to repeat.

for.cpp

```
for (int i = 0; i < 5; i++) {
    cout << i;
}
```

- Syntax: `for(start; stop; step){ }`
- A missing stop condition creates an **infinite for loop**.

### while Loop

📌 Definition

A `while` loop repeats a block of code as long as its condition stays true.

**Simple meaning:** Best when you don't know exactly how many times to repeat.

while.cpp

```
int i = 0;
while (i < 5) {
    cout << i;
    i++;
}
```

- Syntax: `while(condition){ }`
- A condition that never becomes false creates an **infinite while loop**.

### do while Loop

📌 Definition

A `do-while` loop runs the code block first, then checks the condition — guaranteeing at least one run.

**Simple meaning:** "Do it once no matter what, then keep checking."

do-while.cpp

```
int i = 0;
do {
    cout << i;
    i++;
} while (i < 5);
```

- Syntax: `do{ statement }while(condition);`
- Executes **at least once**, even if the condition is false.
- Don't forget the semicolon after `while(condition)`.

03

## Jump Statements

Jump statements let you control the flow inside a loop directly.

### break

📌 Definition

The `break` statement immediately exits the loop or switch it's inside.

**Simple meaning:** "Stop the loop right now."

break.cpp

```
for (int i = 0; i < 10; i++) {
    if (i == 5) break;
    cout << i;
}
```

### continue

📌 Definition

The `continue` statement skips the current iteration and moves to the next one.

**Simple meaning:** "Skip this round, but keep looping."

continue.cpp

```
for (int i = 0; i < 5; i++) {
    if (i == 2) continue;
    cout << i;
}
```

|Basis|break|continue|
|---|---|---|
|Effect|Exits the loop completely|Skips only the current iteration|
|Loop continues after?|No|Yes|

04

## Nested Loops

A loop can be placed inside another loop — this is how patterns and grids are built.

### Loop Inside Loop

📌 Definition

A nested loop is a loop running completely inside another loop's body.

**Simple meaning:** For every one step of the outer loop, the inner loop runs fully.

nested-loop.cpp

```
for (int i = 1; i <= 3; i++) {
    for (int j = 1; j <= 3; j++) {
        cout << "* ";
    }
    cout << "\n";
}
```

### Pattern Programming

- The **outer loop** usually controls the number of rows.
- The **inner loop** usually controls what's printed in each row.
- Used to build shapes like squares, triangles, and pyramids.

MODULE 04

# Functions

Organize your code into reusable blocks, and control how data moves in and out of them.

01

## Function Basics

Functions let you organize code into reusable blocks instead of repeating it everywhere.

### What is a Function?

📌 Definition

A function is a block of code that performs a specific task and can be reused whenever needed.

**Simple meaning:** A mini-program inside your program that you can call again and again.

- Avoids writing the same code repeatedly.
- Keeps programs organized and easier to read.
- Can be called any number of times.

### Function Declaration

📌 Definition

A function declaration tells the compiler a function's name, return type, and parameters — without its body.

**Simple meaning:** A preview that says "this function exists" before it's actually written.

declaration.cpp

```
int add(int a, int b);
```

Also called a function prototype.

### Function Definition

📌 Definition

A function definition contains the actual body — the code that runs when the function is called.

**Simple meaning:** The real instructions inside the function.

definition.cpp

```
int add(int a, int b) {
    return a + b;
}
```

### Function Calling

📌 Definition

Calling a function means executing its code by writing its name followed by parentheses.

**Simple meaning:** "Running" the function whenever you need its task done.

call.cpp

```
int result = add(5, 3);
```

### Return Type

📌 Definition

The return type tells the compiler what kind of value a function sends back to the caller.

**Simple meaning:** The "label" on the box the function hands back.

- `int`, `double`, `string` — the function returns a value of that type.
- `void` — the function returns nothing.
- Use the **return** keyword to send the value back.

02

## Function Features

How arguments are passed to a function changes what happens to the original variables.

### Call by Value

📌 Definition

Call by value passes a copy of the variable to the function — changes made inside don't affect the original.

**Simple meaning:** The function gets a photocopy, not the real thing.

call-by-value.cpp

```
void update(int x) {
    x = 100; // original stays unchanged
}
```

### Call by Reference

📌 Definition

Call by reference passes the actual variable to the function — changes made inside affect the original.

**Simple meaning:** The function gets direct access to the real variable.

call-by-reference.cpp

```
void update(int& x) {
    x = 100; // original changes too
}
```

|Basis|Call by Value|Call by Reference|
|---|---|---|
|What's passed|A copy of the variable|The variable itself|
|Original affected?|No|Yes|
|Syntax|`int x`|`int& x`|

### Default Arguments

📌 Definition

A default argument is a value automatically used for a parameter when the caller doesn't provide one.

**Simple meaning:** A backup value the function falls back on.

default-args.cpp

```
void greet(string name = "Guest") {
    cout << "Hello " << name;
}
```

- Default arguments must be assigned from **right to left**.
- Once one parameter has a default value, every parameter after it must too.

MODULE 05

# Arrays

Store and organize multiple values of the same type, in one dimension and two.

01

## One-Dimensional Arrays

Arrays let you store many values of the same type under a single name.

### Need of a Data Structure

📌 Definition

A data structure is a way of organizing and storing data so it can be used efficiently.

**Simple meaning:** A smart container built for a specific kind of job.

- Storing 100 values as 100 separate variables is unmanageable.
- Data structures group related data together.
- Different problems need different structures.

### Types of Data Structures

|Structure|What It Does|
|---|---|
|Array|Stores same-type elements in contiguous memory|
|String|A sequence of characters|
|Linked List|Elements connected using pointers|
|Queue|First-In, First-Out (FIFO)|
|Stack|Last-In, First-Out (LIFO)|
|Tree|Hierarchical, branching structure|
|Graph|Nodes connected by edges|

### Array Initialisation

📌 Definition

Initializing an array means giving its elements starting values at the time of declaration.

**Simple meaning:** Filling the boxes with values right when you create them.

array-init.cpp

```
int arr[5] = {1, 2, 3, 4, 5};
```

### Array Traversal / Iteration

📌 Definition

Traversal means visiting each element of the array one by one, usually using a loop.

**Simple meaning:** Walking through every box, one at a time.

traversal.cpp

```
for (int i = 0; i < 5; i++) {
    cout << arr[i];
}
```

### Garbage Values

- An uninitialized array element holds a **garbage value**, just like a regular variable.
- Always initialize arrays before reading from them.

### sizeof Operator

📌 Definition

For an array, `sizeof(arr)` returns the total bytes it occupies — not the number of elements.

**Simple meaning:** Total space used by all boxes combined.

sizeof-array.cpp

```
int count = sizeof(arr) / sizeof(arr[0]);
```

Dividing total size by one element's size gives the number of elements.

### Array–Pointer Relation

📌 Definition

An array's name represents the memory address of its first element — it behaves like a pointer.

**Simple meaning:** `arr` and `&arr[0]` point to the same place.

- `arr[i]` is the same as `*(arr + i)`
- The array name itself cannot be reassigned to point elsewhere.

### Undefined Behavior

- Accessing an index outside the array's valid range causes **undefined behavior**.
- The result is unpredictable — it may print garbage, crash, or seem to "work" incorrectly.

### Default Values

- **Global / static** arrays are automatically set to 0.
- **Local** arrays are **not** automatically initialized — they hold garbage values.

### Enhanced for Loop

📌 Definition

The enhanced (range-based) for loop traverses every element of an array without using an index variable.

**Simple meaning:** A shorter way to loop through "each item" directly.

enhanced-for.cpp

```
for (int x : arr) {
    cout << x;
}
```

02

## Two-Dimensional Arrays

A 2D array stores data in rows and columns — like a table or a grid.

### What is a 2D Array?

📌 Definition

A 2D array is an array of arrays — data arranged into rows and columns.

**Simple meaning:** Think of a spreadsheet grid, or a matrix.

### Declaration & Initialization

2d-array.cpp

```
int matrix[2][3] = {
    {1, 2, 3},
    {4, 5, 6}
};
```

First bracket = number of rows, second bracket = number of columns.

### Input & Output

2d-io.cpp

```
for (int i = 0; i < 2; i++)
    for (int j = 0; j < 3; j++)
        cin >> matrix[i][j];
```

### Memory Representation

📌 Definition

In memory, a 2D array is stored as one continuous block, row after row — this is called row-major order.

**Simple meaning:** All of row 0 comes first, then all of row 1, and so on.

### Passing 2D Arrays to Functions

📌 Definition

When passing a 2D array to a function, you must specify the number of columns in the parameter.

**Simple meaning:** The compiler needs the column count to calculate memory offsets correctly.

pass-2d.cpp

```
void printMatrix(int arr[][3], int rows) {
    // rows known, columns fixed at 3
}
```

MODULE 06

# Strings

Work with text — the old C-style way, and the modern string class way.

01

## C-Style Strings

Before the string class, C++ inherited strings from C — plain character arrays.

### Character Array

📌 Definition

A C-style string is an array of characters ending with a special null character `'\0'`.

**Simple meaning:** A row of letter-boxes with an invisible "stop here" marker at the end.

char-array.cpp

```
char name[] = "Hi"; // stored as 'H','i','\0'
```

### Input using cin

- `cin >> name;` reads a C-string.
- It stops reading at the first **space**.

### Input using cin.getline(name, size)

📌 Definition

`cin.getline()` reads a full line into a character array, including spaces, up to a given size limit.

**Simple meaning:** Use it when the text has multiple words.

cin-getline.cpp

```
cin.getline(name, 50);
```

### String Functions

|Function|What It Does|
|---|---|
|`strlen(str)`|Returns the length of the string|
|`strcpy(dest, src)`|Copies one string into another|
|`strcat(str1, str2)`|Joins two strings together|
|`strcmp(str1, str2)`|Compares two strings — returns 0 if equal|

### Problems with C Strings

- Fixed size — cannot grow automatically.
- Needs manual memory handling.
- Easy to accidentally overflow the buffer.
- No built-in safety checks.

02

## String Class

The `string` class makes working with text far easier and safer than character arrays.

### string Library

📌 Definition

The `string` class provides a modern, flexible way to store and manipulate text in C++.

**Simple meaning:** A smarter, self-managing version of a character array.

string-lib.cpp

```
#include <string>
```

### Input using cin

string-cin.cpp

```
string name;
cin >> name; // still stops at a space
```

### Input using getline

string-getline.cpp

```
getline(cin, name); // reads the full line
```

### String Traversal

string-traversal.cpp

```
for (char c : name) {
    cout << c;
}
```

### length() / size()

- Both return the number of characters in the string.
- They do exactly the same thing — use whichever you prefer.

### Concatenation (+)

concat.cpp

```
string full = first + " " + last;
```

### Comparison

Strings can be compared directly with `==`, `!=`, `<`, `>` — comparison follows dictionary order.

### Memory Representation

The `string` class manages its own memory — it automatically grows and shrinks as needed, unlike a fixed-size character array.

### Common Methods

|Method|What It Does|
|---|---|
|`.length()`|Returns the number of characters|
|`.append(str)`|Adds text to the end|
|`.push_back(c)`|Adds one character to the end|
|`.pop_back()`|Removes the last character|
|`.insert(i, str)`|Inserts text at a given position|
|`.erase(pos, count)`|Removes characters starting at a position|
|`.substr(start, len)`|Extracts part of the string|
|`.find(sub)`|Finds the position of a substring|
|`.replace(start, count, str)`|Replaces part of the string|
|`.compare(str)`|Compares two strings|
|`.swap(str)`|Swaps contents with another string|

### char[] vs string

|Basis|char[]|string|
|---|---|---|
|Type|C-style string|C++ string class|
|Size|Fixed|Dynamic|
|End marker|Uses `\0`|Managed automatically|
|Operations|Difficult|Easy|
|Speed|Faster|More convenient|

MODULE 07

# Pointers

Understand memory addresses directly — the foundation for dynamic memory and data structures.

01

## Pointer Basics

A pointer gives you direct access to where data actually lives in memory.

### Why Pointers?

- Allow direct access to memory addresses.
- Enable dynamic memory allocation.
- Let functions modify the original variable (call by reference).
- Essential for arrays, strings, and data structures.

### Memory Address

📌 Definition

Every variable is stored somewhere in memory, and that location is called its address.

**Simple meaning:** Like a house number for a variable.

### Address Of Operator (&)

📌 Definition

The `&` operator returns the memory address of a variable.

**Simple meaning:** "Where does this variable live?"

address-of.cpp

```
cout << &num;
```

### Pointer Variables

📌 Definition

A pointer is a variable that stores the memory address of another variable.

**Simple meaning:** A variable whose "value" is someone else's address.

### Pointer Declaration & Initialization

pointer-init.cpp

```
int num = 10;
int* ptr = &num;
```

### Dereferencing Operator (*)

📌 Definition

The `*` operator accesses the value stored at the address a pointer points to.

**Simple meaning:** "Go to that address, and give me what's there."

dereference.cpp

```
cout << *ptr; // prints 10
```

### Pointer Memory Representation

📦**num**value = 10

←points to

📍**ptr**stores address of num

02

## Pointer Operations

Pointers support their own set of operations, separate from normal variables.

### Pointer Arithmetic

📌 Definition

Pointer arithmetic moves a pointer forward or backward based on the size of the data type it points to.

**Simple meaning:** Adding 1 to a pointer jumps it to the next element, not the next byte.

|Operation|Effect|
|---|---|
|`ptr++`|Moves to the next element|
|`ptr--`|Moves to the previous element|
|`ptr + n`|Moves forward by n elements|
|`ptr - n`|Moves backward by n elements|

### Comparing Pointers

Two pointers can be compared with `==`, `!=`, `<`, `>` — useful for checking if they point to the same location.

### Size of Pointer

`sizeof(ptr)` returns the size of the pointer itself (commonly 8 bytes on 64-bit systems) — not the size of the data it points to.

03

## Pointers and Functions

Pointers let functions reach outside their own scope and modify the caller's variables.

### Call By Reference using Pointers

ptr-call.cpp

```
void update(int* ptr) {
    *ptr = 100;
}
```

### Returning Pointers from Functions

📌 Definition

A function can return a pointer, giving the caller direct access to a variable in memory.

**Simple meaning:** Handing back an address instead of a value.

- Never return the address of a local variable — it's destroyed once the function ends.
- Safe to return addresses of static or dynamically allocated variables.

### Return Multiple Values from Function

📌 Definition

Since a function can only directly return one value, pointers let it update several variables through their addresses instead.

**Simple meaning:** Pass in several addresses, and the function fills them all in.

04

## Pointers and Arrays

Arrays and pointers are closely linked in C++ — an array name is essentially a pointer.

### Array Name as Base Address

📌 Definition

An array's name represents the memory address of its very first element.

**Simple meaning:** `arr` is the same as `&arr[0]`.

### Accessing Array Elements using Pointers

ptr-access.cpp

```
cout << *(arr + i); // same as arr[i]
```

### Array Traversal using Pointers

ptr-traverse.cpp

```
for (int* p = arr; p < arr + 5; p++) {
    cout << *p;
}
```

### Relationship Between Arrays and Pointers

- `arr[i]` and `*(arr + i)` mean the same thing.
- The array name is a constant pointer — it cannot be reassigned to point elsewhere.

05

## Advanced Pointers

A few special pointer types cover cases beyond a standard pointer.

### Null Pointer

📌 Definition

A null pointer points to nothing — it shows that a pointer doesn't currently reference valid memory.

**Simple meaning:** An "empty" pointer.

null-ptr.cpp

```
int* ptr = nullptr;
```

### Void Pointer

📌 Definition

A void pointer can point to any data type, but cannot be dereferenced directly without casting.

**Simple meaning:** A generic pointer — no fixed type attached.

void-ptr.cpp

```
void* ptr;
```

### Double Pointer

📌 Definition

A double pointer is a pointer that stores the address of another pointer.

**Simple meaning:** A pointer pointing to a pointer.

double-ptr.cpp

```
int** ptr2 = &ptr;
```

MODULE 08

# Dynamic Memory Allocation

Request and release memory manually, while your program is running.

01

## Dynamic Memory Allocation

C++ lets you request and release memory manually, while the program is running.

### new Operator

📌 Definition

The `new` operator allocates memory on the heap while the program is running.

**Simple meaning:** Asks the system for a fresh block of memory, on demand.

new.cpp

```
int* ptr = new int(10);
```

### delete Operator

📌 Definition

The `delete` operator frees memory that was allocated with `new`, returning it to the system.

**Simple meaning:** Gives the borrowed memory back.

delete.cpp

```
delete ptr;
```

### Dynamic Arrays

📌 Definition

A dynamic array is created at runtime using `new[]`, letting the size be decided while the program runs.

**Simple meaning:** An array whose size doesn't need to be fixed in advance.

dynamic-array.cpp

```
int* arr = new int[5];
delete[] arr;
```

Arrays created with `new[]` must be freed with `delete[]`, not plain `delete`.

### Memory Leaks

📌 Definition

A memory leak happens when dynamically allocated memory is never freed with `delete`.

**Simple meaning:** Borrowed memory that's never returned — it stays locked away, unused.

- Every `new` should be paired with a matching `delete`.
- Every `new[]` should be paired with `delete[]`.
- Leaks build up over time and can slow down or crash long-running programs.

### Heap vs Stack

|Basis|Stack|Heap|
|---|---|---|
|Allocation|Automatic|Manual (new / delete)|
|Speed|Faster|Slower|
|Size|Limited|Large|
|Lifetime|Ends when scope ends|Until explicitly deleted|
|Managed by|Compiler|Programmer|

MODULE 09

# Structures & Unions

Group different types of data together — structures, unions, enums, and type aliases.

01

## Structures

A structure lets you group related variables of different types under a single name.

### Why Structure?

- Groups different types of variables under one name.
- Makes related data easier to manage and pass around together.

### Structure (struct)

📌 Definition

A structure is a user-defined data type that groups different types of variables under a single name.

**Simple meaning:** A custom box that can hold several different kinds of values together.

struct.cpp

```
struct Student {
    string name;
    int age;
};
```

### Creating Structures

struct-create.cpp

```
Student s1;
s1.name = "Raj";
s1.age = 20;
```

### Arrays of Structures

📌 Definition

An array of structures stores multiple structure variables together — useful for managing many records of the same kind.

**Simple meaning:** A list of Students, not just one.

struct-array.cpp

```
Student students[3];
```

02

## Union

A union looks similar to a structure, but works very differently in memory.

### Union

📌 Definition

A union is a user-defined data type in which all members share the same memory location.

**Simple meaning:** Different labels for the same one storage slot — only one can hold a valid value at a time.

union.cpp

```
union Data {
    int i;
    float f;
};
```

### Difference between Struct and Union

|Basis|Struct|Union|
|---|---|---|
|Memory|Separate for each member|Shared among all members|
|Size|Sum of all members|Size of the largest member|
|Access|All members usable at once|Only one member valid at a time|

03

## Enumerations

Enums give meaningful names to a fixed set of integer constants.

### enum

📌 Definition

An enum is a user-defined type that represents a collection of named integer constants.

**Simple meaning:** Readable names standing in for plain numbers.

enum.cpp

```
enum Day { MON, TUE, WED };
```

Default values start from 0 and increase by 1 unless specified otherwise.

### enum class

📌 Definition

An `enum class` is a scoped, type-safe version of enum introduced in modern C++.

**Simple meaning:** A stricter enum that avoids accidental name clashes.

enum-class.cpp

```
enum class Day { MON, TUE, WED };
```

### enum vs enum class

|Basis|enum|enum class|
|---|---|---|
|Style|C style|Modern C++|
|Scope|Global|Scoped|
|Type safety|Not type safe|Type safe|
|int conversion|Implicit|No implicit conversion|
|Access|`MON`|`Day::MON`|

04

## typedef & using Alias

Both give an existing data type a new, more convenient name.

### typedef

📌 Definition

`typedef` is used to create another name (alias) for an existing data type.

**Simple meaning:** A nickname for a type.

typedef.cpp

```
typedef unsigned long ulong;
```

### using Alias

📌 Definition

The `using` keyword also creates a type alias — it is the modern replacement for `typedef`.

**Simple meaning:** Same job as typedef, cleaner syntax.

using-alias.cpp

```
using ulong = unsigned long;
```

Object Oriented Programming

MODULE 10

# Classes & Objects

The foundation of OOP — how classes, objects, and access modifiers actually work.

01

## OOPS Introduction

Object-Oriented Programming is a completely different way of thinking about code — built around objects instead of just functions.

### Why OOP?

- Models real-world entities as objects in code.
- Makes large programs easier to organize and manage.
- Encourages reusable, secure, well-structured code.

### What is a Programming Paradigm?

📌 Definition

A programming paradigm is a style or approach used to structure and write code.

**Simple meaning:** A "way of thinking" about how to solve problems with code.

### Types of Programming

|Paradigm|Approach|
|---|---|
|Imperative (Procedural)|Step-by-step instructions, organized into functions|
|Functional|Code built from pure functions, avoiding shared state|
|Object-Oriented|Code organized around objects that hold data and behavior|

### Problems with Procedural Programming

- Data and functions are separate — data isn't well protected.
- Hard to manage as the codebase grows large.
- Difficult to reuse code across different parts of a project.

### Special About OOP

♻️**Code Reusability**Write once, reuse everywhere.

🏗️**Manage Large Projects**Organized into clear objects.

🔒**Better Security**Data hidden and controlled.

🛠️**Easy Maintenance**Changes stay contained.

### Features of OOP

|Feature|What It Means|
|---|---|
|Class & Object|The blueprint, and the real thing built from it|
|Encapsulation|Bundling data and functions together, hiding details|
|Abstraction|Showing only essential features, hiding complexity|
|Inheritance|Reusing properties from an existing class|
|Polymorphism|One action, many forms|

02

## Class

A class is where OOP begins — the blueprint every object is built from.

### What is a Class?

📌 Definition

A class is a user-defined data type that acts as a blueprint for creating objects.

**Simple meaning:** A template — like a house blueprint, not the house itself.

### Creating a Class

class.cpp

```
class Car {
    public:
        string brand;
        void honk() { cout << "Beep!"; }
};
```

### Data Members

📌 Definition

Data members (attributes / fields) are the properties that describe an object.

**Simple meaning:** The "what it has" — like `brand` for a Car.

### Member Functions

📌 Definition

Member functions (behaviour / methods) are the operations that can be performed on an object.

**Simple meaning:** The "what it can do" — like `honk()` for a Car.

03

## Object

An object is the real, usable thing built from a class's blueprint.

### Instance of a Class

📌 Definition

An object is an instance of a class — a real entity created using the class blueprint.

**Simple meaning:** The actual house, built from the blueprint.

### Creating Objects

|Type|Where It Lives|Example|
|---|---|---|
|Static Object|Stack|`Car c1;`|
|Dynamic Object|Heap (using `new`)|`Car* c2 = new Car();`|

### Memory Representation of Objects

Each object gets its own copy of the data members, but member functions are shared across all objects of the class.

### Object vs Class

|Basis|Class|Object|
|---|---|---|
|What it is|Blueprint|The actual building|
|Memory|No memory allocated|Takes up memory|
|Count|One class|Many objects possible|

04

## Access Modifiers

Access modifiers control who is allowed to see or use a class's members.

|Modifier|Accessible From|
|---|---|
|public|Anywhere — global level|
|private|Only inside the same class|
|protected|Inside the class and its derived classes|

MODULE 11

# Constructors

The special function that sets up an object the instant it's created.

01

## Constructors

A constructor is a special function that sets up an object the moment it's created.

### What is a Constructor?

📌 Definition

A constructor is a special function that is automatically called when an object is created.

**Simple meaning:** The "setup crew" that prepares a new object.

- Name must be exactly the same as the class name.
- Has no return type — not even `void`.
- Called automatically — never invoked manually.
- Cannot be static, virtual, or inherited.

### Default Constructor

📌 Definition

A default constructor takes no parameters and is called automatically when no values are provided.

**Simple meaning:** The "blank" setup, with no custom input.

default-constructor.cpp

```
class Car {
    public:
        Car() { cout << "Car created"; }
};
```

### Parameterised Constructor

📌 Definition

A parameterised constructor accepts arguments, letting you set initial values when creating an object.

**Simple meaning:** A "custom" setup, using values you provide.

param-constructor.cpp

```
Car(string b) { brand = b; }
```

### this Keyword

📌 Definition

`this` is a pointer that refers to the current object calling the function.

**Simple meaning:** "Me" — the object talking about itself.

this.cpp

```
Car(string brand) {
    this->brand = brand; // distinguishes member from parameter
}
```

### Copy Constructor

📌 Definition

A copy constructor creates a new object by copying the data of an already existing object.

**Simple meaning:** Making a duplicate of an existing object.

copy-constructor.cpp

```
Car c2 = c1; // copy constructor called
```

### Shallow Copy vs Deep Copy

|Basis|Shallow Copy|Deep Copy|
|---|---|---|
|What's copied|Only the pointer/reference|The actual data being pointed to|
|Shared memory?|Yes — risky|No — fully independent|

### Constructor Overloading

📌 Definition

Constructor overloading means having multiple constructors in the same class with different parameters.

**Simple meaning:** Several different "setup styles" for the same class.

### Member Function Outside the Class

📌 Definition

A member function can be defined outside the class body using the scope resolution operator.

**Simple meaning:** Declare it inside the class, write its code outside.

outside-class.cpp

```
void Car::honk() {
    cout << "Beep!";
}
```

Syntax: `returnType className::methodName` — the method must still be declared inside the class first.

### Initialisation List

📌 Definition

An initialisation list assigns values to data members directly, before the constructor body runs.

**Simple meaning:** A faster way to set starting values.

init-list.cpp

```
Car(string b) : brand(b) { }
```

MODULE 12

# Destructor

The clean-up function that runs right before an object is destroyed.

MODULE 13

# Encapsulation

Wrapping data and functions together, and protecting them from outside interference.

MODULE 14

# Static Members

Data and functions that belong to the class itself, not to any one object.

01

## Destructor

A destructor is the counterpart to a constructor — it cleans up an object right before it's destroyed.

### Object Life Cycle

🏗️**Constructor**object created

→

⚙️**Object in Use**lifetime

→

🧹**Destructor**object destroyed

### Destructor Syntax

📌 Definition

A destructor is a special function automatically called when an object goes out of scope or is deleted.

**Simple meaning:** The "clean-up crew" before an object disappears.

destructor.cpp

```
~Car() { cout << "Car destroyed"; }
```

- Same name as the class, prefixed with `~`
- Takes no parameters and returns nothing.
- Only one destructor is allowed per class — it cannot be overloaded.

02

## Encapsulation

Encapsulation wraps data and the functions that use it into one protected unit.

### The Problem

Without protection, any part of a program can directly change an object's data — leading to invalid or unsafe states.

### Getter & Setter

📌 Definition

Getters and setters are public functions used to safely read and modify private data.

**Simple meaning:** Controlled doors into otherwise locked data.

getter-setter.cpp

```
int getAge() { return age; }
void setAge(int a) { age = a; }
```

### Data Hiding

📌 Definition

Data hiding means restricting direct access to a class's internal data, usually with the `private` keyword.

**Simple meaning:** Locking the data away from outside interference.

### Encapsulation

📌 Definition

Encapsulation is the wrapping of data members and member functions into a single unit — the class.

**Simple meaning:** Bundling the "what it has" and "what it does" together.

### Encapsulation vs Data Hiding

|Basis|Encapsulation|Data Hiding|
|---|---|---|
|What it does|Bundles data + functions together|Restricts access to that data|
|Scope|Broader concept|A part of encapsulation|

### Benefits

🔒**Data Security**Protects sensitive information.

🎛️**Controlled Access**Only through defined methods.

🛠️**Easy Maintenance**Internals can change safely.

📖**Read-Only Classes**Skip the setter to lock a value.

03

## Static Members

Static members belong to the class itself, not to any single object.

### Why Static?

- Avoids duplicating the same data for every object.
- Shares common data across all objects.
- Belongs to the class, not an individual object.

### Static Variables

📌 Definition

A static variable is shared by all objects of a class — only one copy exists for the entire class.

**Simple meaning:** One shared box, instead of a separate box per object.

static-var.cpp

```
static int count;                         // declaration
int Car::count = 0;                   // initialisation, outside the class
```

- Initialised outside the class.
- Can be accessed using the class name directly.

### Static Function

📌 Definition

A static function belongs to the class and can be called without creating any object.

**Simple meaning:** A class-level action, not tied to a specific object.

- Invoked using the class name.
- Can access only other static members.
- Cannot use the `this` pointer.

MODULE 15

# Inheritance

Reusing a class's properties and behavior in a new class — and the five patterns for doing it.

01

## Inheritance Basics

Inheritance lets one class reuse the properties and functions of another.

### Why Inheritance?

- Reuses existing code instead of writing it again.
- Reduces code duplication.
- Makes code easier to maintain.

### Parent (Base) Class

📌 Definition

The parent (base) class is the class whose properties and functions are inherited by another class.

**Simple meaning:** The original class being borrowed from.

### Child (Derived) Class

📌 Definition

The child (derived) class inherits the properties and functions of the parent class, and can add its own.

**Simple meaning:** The class that receives the inheritance — and can extend it further.

### Syntax

inheritance.cpp

```
class ChildClass : accessModifier ParentClass
{
    // Child Class
};
```

02

## Types of Inheritance

C++ supports five different patterns for how classes can inherit from one another.

### Single Inheritance

📌 Definition

One parent class is inherited by one child class.

   A
   │
   B

### Multilevel Inheritance

📌 Definition

A chain of inheritance — Parent → Child → Grandchild.

   A
   │
   B
   │
   C

### Hierarchical Inheritance

📌 Definition

One parent class is inherited by multiple child classes.

      A
     / \
    B   C

### Multiple Inheritance

📌 Definition

One child class inherits from multiple parent classes.

   A       B
    \     /
      C

- If both parent classes have a member with the same name, **ambiguity** occurs.
- Resolved using the **Scope Resolution Operator (::)** — e.g. `obj.A::display();`

### Hybrid Inheritance

📌 Definition

A combination of multiple inheritance types used together.

        A
       / \
      B   C
       \ /
        D

03

## Diamond Problem

A specific ambiguity issue that appears in hybrid inheritance.

📌 Definition

The diamond problem occurs in hybrid inheritance when two parent classes inherit from the same base class, causing the child to receive multiple copies of that base class.

**Simple meaning:** The grandparent's data gets duplicated and becomes ambiguous.

### Solutions

|Solution|What It Does|
|---|---|
|Scope Resolution (::)|Specifies exactly which parent's member to use|
|Virtual Inheritance|Ensures only one shared copy of the base class is inherited|

04

## Constructor & Destructor Calling Order

In inheritance, constructors and destructors run in a strict, predictable order.

### Constructor Order

1️⃣**Parent Constructor**

→

2️⃣**Child Constructor**

### Destructor Order

1️⃣**Child Destructor**

→

2️⃣**Parent Destructor**

Destruction always happens in the reverse order of construction.

05

## Access Mode Summary

The inheritance type you choose changes how a parent's members are accessed in the child class.

|Parent Member|Public Inheritance|Protected Inheritance|Private Inheritance|
|---|---|---|---|
|Public|Public|Protected|Private|
|Protected|Protected|Protected|Private|
|Private|Not Accessible|Not Accessible|Not Accessible|

MODULE 16

# Polymorphism

One action, many forms — resolved either at compile time or at run time.

01

## Polymorphism

Polymorphism means "many forms" — the same action behaving differently depending on the context.

📌 Definition

Polymorphism is the ability of a function or operator to behave differently based on the object or data it's working with.

**Simple meaning:** One name, many behaviors.

### Types of Polymorphism

|Type|Resolved|Also Known As|
|---|---|---|
|Compile-Time|At compile time|Static / Early Binding|
|Run-Time|At run time|Dynamic / Late Binding|

**Binding** means connecting a function call with its actual function implementation.

02

## Compile-Time Polymorphism

Achieved through function, constructor, or operator overloading.

### Function Overloading

📌 Definition

Function overloading means having the same function name with different parameters.

**Simple meaning:** One name, several versions, chosen by the arguments used.

- Function name must stay the same.
- Parameters must differ — in number, type, or order.
- Return type alone cannot overload a function.

### Operator Overloading

📌 Definition

Operator overloading redefines how an existing operator behaves for user-defined objects.

**Simple meaning:** Teaching `+` or `==` new tricks for your own classes.

operator-overload.cpp

```
returnType operator operatorSymbol(parameters);
```

- Only existing operators can be overloaded — new ones cannot be created.
- At least one operand must be a user-defined type.
- `::`, `.`, `?:`, and `sizeof` cannot be overloaded.

03

## Run-Time Polymorphism

Achieved through function overriding and virtual functions.

### Function Overriding

📌 Definition

Function overriding is when a child class provides its own implementation of a function already defined in the parent class.

**Simple meaning:** The child rewrites what it inherited.

- Requires both a parent and a child class.
- Function name and parameters must match exactly.
- Achieved through inheritance.

### Virtual Function

📌 Definition

A virtual function tells the compiler to decide, at run time, which version of the function to call — based on the actual object, not the pointer type.

**Simple meaning:** "Wait until run time to decide which version to run."

virtual.cpp

```
virtual void speak();
```

- Declared with the `virtual` keyword in the base class.
- Must be overridden in the derived class.
- Works through a base class pointer or reference.
- Constructors cannot be virtual.
- Static member functions cannot be virtual.

|Basis|Static Binding|Dynamic Binding|
|---|---|---|
|Decision based on|Pointer / reference type|The actual object being pointed to|
|Also called|Early binding|Late binding|

The `override` keyword is optional, but makes overriding intent explicit.

MODULE 17

# Abstraction

Hiding complexity and exposing only what the user actually needs.

MODULE 18

# Exception Handling

Responding gracefully to runtime errors instead of letting the program crash.

01

## Abstraction

Abstraction is about showing only what matters, and hiding the messy details.

📌 Definition

Abstraction means hiding implementation details and showing only the essential features.

**Simple meaning:** You see the steering wheel, not the engine wiring.

|Type|Meaning|
|---|---|
|Partial Abstraction|Some details hidden, some visible|
|Complete Abstraction|All implementation details hidden|

02

## Partial Abstraction

Achieved using regular classes with private members.

📌 Definition

Partial abstraction hides some data (using private members) while still exposing some parts publicly.

**Simple meaning:** Some parts locked away, some parts open.

03

## Abstract Class

A class specifically designed to be incomplete, forcing derived classes to finish it.

📌 Definition

An abstract class is a class that contains at least one pure virtual function and cannot be used to create objects.

**Simple meaning:** A blueprint that's intentionally incomplete.

- Contains at least one pure virtual function.
- Cannot create objects of an abstract class directly.
- Can still have constructors.
- Can contain normal member functions and data members.

04

## Pure Virtual Function

The function that makes a class abstract in the first place.

📌 Definition

A pure virtual function has no implementation in the base class and must be overridden in the derived class.

**Simple meaning:** A function that's declared but deliberately left empty.

pure-virtual.cpp

```
virtual returnType functionName(parameters) = 0;
```

- Declared using `= 0`.
- Must be overridden in the derived class.
- If not overridden, the child class also becomes abstract.

05

## Interface in C++

C++ doesn't have a dedicated "interface" keyword — it's simulated using abstract classes.

📌 Definition

An interface is an abstract class that contains only pure virtual functions, used to define a contract for derived classes.

**Simple meaning:** A promise every derived class must fulfill.

- Contains only pure virtual functions.
- Cannot create objects from it.
- Defines a strict contract for derived classes.
- Supports implementing multiple interfaces.

### Abstraction vs Encapsulation

|Basis|Abstraction|Encapsulation|
|---|---|---|
|Focus|Hiding complexity|Hiding data|
|Achieved via|Abstract classes, interfaces|Access modifiers (private/public)|

06

## Exception Handling

Exception handling lets a program respond gracefully to runtime errors instead of crashing.

### Error vs Exception

|Basis|Error|Exception|
|---|---|---|
|Recoverable?|Usually not|Yes, can be handled|
|When it occurs|Compile time or serious runtime failure|Runtime, expected to be caught|

### What is Exception Handling?

📌 Definition

Exception handling is a mechanism to detect and respond to runtime errors without crashing the program.

**Simple meaning:** A safety net for things going wrong while the program runs.

### Keywords

|Keyword|Role|
|---|---|
|`try`|Wraps the risky code that might fail|
|`throw`|Signals that an exception has occurred|
|`catch`|Handles the thrown exception|

try-catch.cpp

```
try {
    throw 1;
} catch (int e) {
    cout << "Caught: " << e;
}
```

- Risky code goes inside `try`.
- `throw` raises the exception.
- One `try` block can have multiple `catch` blocks.
- `catch(...)` catches every type of exception.

MODULE 19

# Standard Template Library (STL)

Ready-made containers, iterators, and algorithms that ship with C++.

01

## STL Introduction

The Standard Template Library is a collection of ready-made, reusable tools that ship with C++.

📌 Definition

STL (Standard Template Library) is a collection of pre-built classes and functions for common data structures and algorithms.

**Simple meaning:** A toolbox that saves you from building common data structures from scratch.

### Components of STL

📦**Containers**Store collections of data.

🧭**Iterators**Traverse through containers.

⚙️**Algorithms**Perform operations on containers.

02

## Vector

A dynamic array that resizes itself automatically.

📌 Definition

A vector is a dynamic array that can grow and shrink automatically during runtime.

**Simple meaning:** An array that never runs out of room.

vector.cpp

```
#include <vector>
vector<int> v;
```

### Common Functions

|Function|What It Does|
|---|---|
|`push_back()`|Adds an element at the end|
|`pop_back()`|Removes the last element|
|`size()`|Returns the number of elements|
|`empty()`|Returns true if there are no elements|
|`clear()`|Removes all elements|
|`front()`|Returns the first element|
|`back()`|Returns the last element|
|`at(index)`|Returns the element at index, with bounds checking|

03

## Pair

A simple container that bundles exactly two values together.

📌 Definition

A pair is a container that stores two values together, of possibly different types.

**Simple meaning:** A two-item bundle.

pair.cpp

```
#include <utility>
pair<int, string> p;
```

- `.first` stores the first value.
- `.second` stores the second value.

04

## Set & Unordered Set

Both store unique elements — but with very different internal behavior.

### Set

📌 Definition

A set stores unique elements in sorted order.

**Simple meaning:** No duplicates allowed, always kept sorted.

set.cpp

```
#include <set>
set<int> s;
```

### Unordered Set

📌 Definition

An unordered set stores unique elements without maintaining any order, using a hash table internally.

**Simple meaning:** No duplicates, no guaranteed order — but faster.

unordered-set.cpp

```
#include <unordered_set>
unordered_set<int> us;
```

### Common Functions (both)

|Function|What It Does|
|---|---|
|`insert()`|Adds an element (duplicates ignored)|
|`erase()`|Removes an element|
|`find()`|Returns an iterator to an element if found|
|`count()`|Returns 1 if the element exists, else 0|
|`size()`|Returns the number of elements|
|`empty()`|Returns true if there are no elements|

### Set vs Unordered Set

|Basis|Set|Unordered Set|
|---|---|---|
|Order|Sorted|Unsorted|
|Internal structure|Tree-based|Hash-table based|
|Speed|Slower|Faster (average)|

05

## Map & Unordered Map

Both store key-value pairs — the same sorted-vs-hashed distinction as sets.

### Map

📌 Definition

A map stores data as key-value pairs, where keys are unique and kept sorted.

**Simple meaning:** A dictionary — look up a value using its key.

map.cpp

```
#include <map>
map<int, string> mp;
```

### Unordered Map

📌 Definition

An unordered map stores key-value pairs without maintaining any order, using a hash table internally.

**Simple meaning:** Same dictionary idea, no order, faster lookups.

unordered-map.cpp

```
#include <unordered_map>
unordered_map<int, string> ump;
```

### Common Functions (both)

|Function|What It Does|
|---|---|
|`insert({key, value})`|Adds a key-value pair|
|`erase()`|Removes a pair using its key|
|`find()`|Searches for a key|
|`count()`|Returns 1 if the key exists, else 0|
|`size()`|Returns the number of pairs|
|`empty()`|Returns true if there are no pairs|
|`[key]`|Accesses or updates a value by key|

If the key doesn't exist, the `[]` operator creates it with a default value.

### Map vs Unordered Map

|Basis|Map|Unordered Map|
|---|---|---|
|Keys|Sorted|Unsorted|
|Internal structure|Tree-based|Hash-table based|
|Speed|Slower|Faster (average)|

06

## Iterators

Iterators are how you move through the elements inside any STL container.

📌 Definition

An iterator is an object used to traverse the elements of a container.

**Simple meaning:** A pointer-like tool that walks through a container, one element at a time.

iterator.cpp

```
vector<int>::iterator it;
```

### Functions

|Function|What It Does|
|---|---|
|`begin()`|Points to the first element|
|`end()`|Points just past the last element|
|`rbegin()`|Points to the last element (reverse)|
|`rend()`|Points just before the first element (reverse)|

`auto` lets the compiler automatically determine the data type of a variable from its value — handy for long iterator types.

07

## Algorithms

Ready-made STL functions that operate on containers, so you don't have to write them yourself.

📌 Definition

Algorithms are pre-defined STL functions used to perform common operations on containers.

**Simple meaning:** Common tasks like sorting or searching, already written for you.

algorithm.cpp

```
sort(v.begin(), v.end());
```

### Common Algorithms

|Function|What It Does|
|---|---|
|`sort()`|Sorts elements in ascending order by default|
|`reverse()`|Reverses the order of elements|
|`swap()`|Swaps the values of two variables|
|`max() / min()`|Returns the larger / smaller of two values|
|`max_element()`|Returns an iterator to the largest element|
|`min_element()`|Returns an iterator to the smallest element|
|`find()`|Searches for a value in a range|
|`count()`|Counts occurrences of a value|
|`binary_search()`|Checks if a value exists (needs a sorted container)|
|`lower_bound()`|Returns an iterator to the first element ≥ value|
|`upper_bound()`|Returns an iterator to the first element > value|