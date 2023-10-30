---
Created: 2023-06-24
Type: Programming Note
Programming Language: "[[Rust MOC]]"
Related: 
Completed: true
---
---
## Definition
Shadowing allows a [[Rust Variables and Constants|variable]] to be re-declared in the same [[Rust Scope|scope]] with the same name

---
### Case 1: Variable re-declared in a different scope
- when we exit the scope the original variable stay intact
```rust
let x = 5;
{
	let x = "ciao";
	println!("{x}"); // Output: ciao
}

println!("{x}");     // Output: 5
```

### Case 2: Variable re-declares in the same scope
- The original variable it's overwritten by the new one
```rust
let x = 5;
println!("{x}"); // Output: 5
    
let x = "ciao";
println!("{x}"); // Output: ciao
```


>[!warning] Nota:
>We are not [[Rust variables mutation|mutating]] the original variable but we a declaaring a new variable we the same name of the old one 

**Example of re-declaration:**
``` rust
let x = 5;
let x = "Hello";
```

**Example of mutation:**
``` rust
let mut x = 5;
x = 6;
```

