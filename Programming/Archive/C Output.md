Completed: Yes
Created: March 21, 2023
Tags: [[C MOC]], [[Programming HUB]]

---
To output values or print text in C, you can use the `printf()` function:
``` C
#include <stdio.h>  
  
int main() {  
  printf("Hello World!");  
  return 0;  
}
```

---
## New Lines
To insert **a new line**, you can use the `\n` character:
``` C
#include <stdio.h>  
  
int main() {  
  printf("Hello World!**\n**");  
  printf("I am learning C.");  
  return 0;  
}
```

**Multiple lines** with a single `printf()`:
``` C
#include <stdio.h>  
  
int main() {  
  printf("Hello World!**\n**I am learning C.**\n**And it is awesome!");  
  return 0;  
}
```

>[! warning] TIP:
> - Two `\n` characters after each other will create a blank line:

### What is `\n` exactly?

The newline character (`\n`) is called an **escape sequence**, and it forces the cursor to change its position to the beginning of the next line on the screen. This results in a new line.

Examples of other valid escape sequences are:
|  Escape Sequence|  Description | Try It|
| --- | --- | --- |
| \\t| Creates a horizontal tab |[Link](https://www.w3schools.com/c/tryc.php?filename=demo_esc_char) |
|   \\\\ |  Inserts a backslash character (\\)|[Link](https://www.w3schools.com/c/tryc.php?filename=demo_esc_char_backslash)|
|\\"|Inserts a double quote character|[Link](https://www.w3schools.com/c/tryc.php?filename=demo_esc_char_dblquote) |
