Tag: [[C MOC]],[[Programming HUB]]

---
Variables are containers for storing data values, like numbers and characters.

## Declaring (Creating) Variables
To create a variable, specify the **[data type](obsidian://open?vault=Main%20Vault&file=Programming%2FArchive%2FC%20Data%20Types)** and assign it a **value**:

### Syntax
```c
type variableName = value;
```

You can also declare a variable without assigning the value, and assign the value later:
```c
// Declare a variable  
int myNum;  
  
// Assign a value to the variable  
myNum = 15;
```

## Variable Names

All C **variables** must be **identified** with **unique names**.
These unique names are called **identifiers**.

**Note:** It is recommended to use descriptive names in order to create understandable and maintainable code:
```c
// Good  
int minutesPerHour = 60;  
  
// OK, but not so easy to understand what **m** actually is  
int m = 60;
```

## Output Variables
You learned from the [output chapter](obsidian://open?vault=Main%20Vault&file=Programming%2FArchive%2FC%20Output) that you can output values/print text with the `printf()` function:

In many other programming languages, you would normally use a print function to display the value of a variable. However, this is **not possible in C**:
```c
int myNum = 15;  
printf(myNum);  // Nothing happens
```

To output variables in C, you must get familiar with something called "[format specifiers](obsidian://open?vault=Main%20Vault&file=Programming%2FArchive%2FC%20Format%20Specifiers)"

### Syntax
```c
printf("format specifier", variable );
```

## Change Variable Values

**Note:** If you assign a new value to an existing variable, it will overwrite the previous value:

```c
int myNum = 15;  // myNum is 15  
myNum = 10;  // Now myNum is 10
```

## Assign Values
You can also assign the value of one variable to another:

```c
int myNum = 15;  
  
int myOtherNum = 23;  
  
// Assign the value of myOtherNum (23) to myNum  
myNum = myOtherNum;  
  
// myNum is now 23, instead of 15
```

---
Sure, here is a brief description of the different variable types commonly used in programming:

1.  Integer variables: These variables store whole numbers without any decimal points. In C, you can use different types of integer variables such as `int`, `short`, `long`, `unsigned int`, etc. The size of these variables depends on the system architecture.
    
2.  Floating-point variables: These variables store real numbers, including numbers with decimal points. In C, you can use two types of floating-point variables, `float` and `double`. `float` can store numbers with up to 7 significant digits, while `double` can store numbers with up to 15 significant digits.
    
3.  Character variables: These variables store a single character such as a letter, digit, punctuation mark, or a whitespace character. In C, you can use the `char` type to define a character variable.
    
4.  Arrays: These variables can store a collection of values of the same data type in a single variable. In C, you can define an array using square brackets, for example: `int myArray[5];`. This will create an array of 5 integers.
    
5.  Pointers: These variables store the memory address of another variable. Pointers are used to access and modify the value of a variable indirectly. In C, you can define a pointer using the `*` operator, for example: `int* myPointer;`. This will create a pointer to an integer variable.
    
6.  Structures: These variables allow you to define your own data types with multiple variables of different data types. In C, you can define a structure using the `struct` keyword, for example:
    

arduinoCopy code

`struct Person {     char name[20];     int age; };`

This will define a structure called `Person` with two variables, `name` and `age`.

7.  Unions: These variables allow you to define a data type that can hold different types of data at different times. In C, you can define a union using the `union` keyword, for example:

arduinoCopy code

`union Data {     int myInt;     float myFloat; };`

This will define a union called `Data` with two variables, `myInt` and `myFloat`.

8.  Enumerations: These variables allow you to define a set of named constants. In C, you can define an enumeration using the `enum` keyword, for example:

arduinoCopy code

`enum Color {     RED,     GREEN,     BLUE };`

This will define an enumeration called `Color` with three named constants, `RED`, `GREEN`, and `BLUE`.