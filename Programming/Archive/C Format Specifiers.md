Tag: [[C MOC]], [[Programming HUB]]

---
In C programming, a format specifier is a special character that is used to specify the type of data that will be printed or read in a formatted input/output operation. 

Format specifiers are used in conjunction with the printf() and scanf() functions to format the input and output of data.

**Here are some commonly used format specifiers in C:**
-   `%d` or `%i` - Used for integers, such as int.
-   `%f` - Used for floating-point numbers, such as *float* or *double*.
-   `%c` - Used for characters, such as *char*.
-   `%s` - Used for *strings*, such as ***char arrays or pointers***.
-   `%p` - Used for *pointers*, such as void*.
-   `%x` or `%X` - Used for *hexadecimal numbers*.

**printf() example:** [[C Output]]
```c
int a = 10; 
float b = 3.14;

printf("The value of a is %d and the value of b is %f", a, b);`
```
In this code, the format specifiers %d and %f are used to print the integer and floating-point values of a and b, respectively.

**scanf() example:**  [[C User Input]]
``` c
   int age;
   char name[20];
   
   printf("Enter your age: ");
   scanf("%d", &age); // using %d format specifier to read integer input
```