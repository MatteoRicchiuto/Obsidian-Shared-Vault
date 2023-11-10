---
Created: 2023-11-06
Type: Uni Note
Class:
  - "[[Progettazione Sistemi Digitali (class)]]"
Academic Year: 2023/2024
Related:
  - "[[Circuiti sequenziali]]"
  - "[[Latch SR]]"
Completed: true
---
---
## Index
1. [[#Definizione]]
2. [[#Circuito]]
3. [[#Variabili]]

---
## Definizione
Il **Gated Latch** è un circuito [[Circuiti sequenziali|sequenziale]] ed [[Circuiti Sincroni ed Asincroni#Circuiti Sincroni|sincrono]] utilizzato per la memorizzazione di un bit

Il suo funzionamento è identico al [[Latch SR]] soltanto che abbiamo anche la variabile di *clock*, quest'ultima ci permette di cambiare lo stato del latch soltanto quando il clock ha valore 1

- S = set
- R = reset
- C = clock
- y = stato (output)

![[IMG_2FFF2751344A-1.jpeg|300]]

---
## Circuito
![[IMG_AFEBED8E6223-1.jpeg|600]]

---
## Stati nel tempo 
*y(t)* = stato presente
*y(t+1)* = stato futuro

![[IMG_C0FD19856A49-1.jpeg|500]]

---