---
Academic Year: 2023/2024
Related:
  - "[[Programmazione Calcolatori (Class)]]"
  - "[[Python MOC]]"
WebSite:
---
---
**Lezioni:**
[[Manipolazione del testo]]

**mkdirs** per creare directory annidate nel modulo os

## Programmazione ad oggetti 

**Programmazione strutturata:**

```list.append(L,4)``` equivalente a ```L.append(4)```

### Class


## yields     

## Generatory Lazy

## Cose strane 
```python
def power_factory(exp):
    def power_func(num):
        return num ** exp
    return power_func

cube_func = power_factory(exp=3)
square_func = power_factory(exp=2)

print(cube_func(3))
print(square_func(5))
```

