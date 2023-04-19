
![[Recording 20230416194632.webm]]
Completed: Yes
Created: March 22, 2023
Tag: [[C MOC]], [[C Funcions]], [[C free Funcion]], [[C malloc Funcion]]

---
## Description

The C library function void ``realloc(void \*ptr, size)`` attempts to resize the memory block pointed to by **ptr** that was previously allocated with a call to **malloc** or **calloc**.

If **there isn’t enough memory space** in the previous position, the function may move the memory block to a new location (whose address is returned by the function).

## Syntax
```c
void *realloc(void *ptr, size)
```

- **ptr** − This is the pointer to a memory block previously allocated with malloc, calloc or realloc to be reallocated. If this is NULL, a new block is allocated and a pointer to it is returned by the function.

- **size** − This is the new size for the memory block, in bytes. If it is 0 and ptr points to an existing block of memory, the memory block pointed by ptr is deallocated and a NULL pointer is returned.

## Return Value

This function returns a pointer to the newly allocated memory, or NULL if the request fails.

## Example

```c

#include <stdio.h>
#include <stdlib.h>

int main () {
   char *str;

   /* Initial memory allocation */
   str = (char *) malloc(15);
   strcpy(str, "tutorialspoint");
   printf("String = %s,  Address = %u\n", str, str);

   /* Reallocating memory */
   str = (char *) realloc(str, 25);
   strcat(str, ".com");
   printf("String = %s,  Address = %u\n", str, str);

   free(str);
   
   return(0);
}
```
**Output:**
```txt
String = tutorialspoint, Address = 355090448
String = tutorialspoint.com, Address = 355090448
```