Completed: Yes
Created: March 27, 2023
Tag: [[C MOC]], [[Programming HUB]]

---
An arithmetic operator performs mathematical operations such as addition, subtraction, multiplication, division etc on numerical values (constants and variables).

|Operator| Meaning of Operator |
|---|---|
| + | addition or unary plus|
| - | subtraction or unary minus|
| * | multiplication |
| / |division |
|% | remainder after division (modulo division) |

**Example:**
``` c
    int a = 9,b = 4, c;
    
    c = a + b; // Output: 13
    c = a - b; // Output: 5
    c = a * b; // Output: 36
    c = a / b; // Output: 2
    c = a % b; // Output: 1
```

>[!warning]
> - The `%` operator can only be used with integers. 
> - When using the `/` operator the result will be an integer if bought the values are integers

## Strange Case
In normal calculation, `9/4 = 2.25`. However, the output is `2` in the program.

It is because **both the variables a and b are integers**. Hence, the output is also an integer. The compiler neglects the term after the decimal point and shows answer `2` instead of `2.25`.

**Example:**
```c
a = 5.0;
b = 2.0;
c = 5;
d = 2; 
// Either one of the operands is a floating-point number
a/b = 2.5  
a/d = 2.5  
c/b = 2.5  

// Both operands are integers
c/d = 2
```