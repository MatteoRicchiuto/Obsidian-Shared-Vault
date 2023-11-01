Status: #Complete
Created: Jul 10, 2023
Academic Year: 2022-2023
Class: [[Logica e Reti Logiche (Class)]]
Macro argomento: [[Logica Proposizionale]]
Type: #Uni/Notes 
Tag: [[Metodo dei Tableaux nella logica del primo ordine]]

---
# Indice:
1. [[#Scopo]]
2. [[#Metodo]]
3. [[#Sviluppare una formula]]
4. [[#α o β]]
5. [[#Chiudere una ramo]]
6. [[#Consigli]]
7. [[Dimostrazione funzionamento metodo Tableaux]]


---
## Scopo
Il metodo dei tableaux è un metodo dimostrativo utilizzato per verificare se una determinata formula è una tautologia.

---
## Metodo 
Per dimostrare che una determinata formula (*F*) è una tautologia dobbiamo vedere se non esiste alcuna [[Logica Proposizionale#Interpretazioni|interpretazione]] che rendere vera la negazione della formula (*¬F*)

1. Negare F
2. Sviluppare F
3. Continuare a [[#Sviluppare una formula|sviluppare]] le semplificazioni (sotto formule) di F 
...
4. Fermarsi quando si è raggiunta la semplificazione massima ho si è riuscito a [[#Chiudere una ramo|chiudere tutti i rami]]

**Fine:** 
- Se **non è** stato possibile chiudere tutti i rami significa che esiste una o più interpretazioni di *¬F* vere quindi *F* non è una tautologia
- Se **è** stato possibile chiudere tutti i rami allora *¬F* è una contraddizione e *F* è una tautologia

---
## Sviluppare una formula
- Sviluppare una formula significa scomporla nelle sotto formule che la compongono
	- es: x ∨ y è composta da x e y 

- Lo sviluppo di una formula o sotto formula può dare due risultati: ![[Screenshot 2023-07-13 at 11.39.06.png]]
1. Uno **"stack"** , generato da una formula *α* (alpha) composta da *α1* e *α2* (sotto-formule) posizionate una sopra all'altra
	- ***oss:*** una formula α si può anche chiamare "formula di tipo AND"
	- 
1. Un **"Ramo"**, generato da una formula *β* (beta) composta da *β1* e *β2* (sotto-formule) che si dividono in due rami
	- oss: una formula β si può anche chiamare "formula di tipo OR"

---
## α o β
![[IMG_79BD37A718E2-1.jpeg]]




---
## Chiudere una ramo
- chiudere un ramo significa non continuare a semplificare (scomporre) un ramo del tableaux perché si è incontrata una contraddizione

***Es:*** ![[Screenshot 2023-07-11 at 10.24.26.png]]

Se si riesce a chiudere tutti i rami allora abbiamo dimostrato che la formula originale è una tautologia

---
## Consigli 
1. Nello svolgimento di un tableaux si ha libertà su quale parte dello stack o quale ramo svolgere prima.
	- Solitamente è più veloce risolvere le formule *α* (AND) rispetto alle formule  *β* (OR), infatti ogni volta che risolviamo una formula *β* (OR) creiamo 2 rami raddoppiando il numero di operazioni necessarie
