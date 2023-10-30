 Status: #NotComplete
Academic Year: 2022-2023
Class: [[Logica e Reti Logiche (Class)]] [[Progettazione Sistemi Digitali (class)]]
Created: Jul 06, 2023
Type: #Uni/Notes

---
## Indice:
**Basi:**
- [[#Funzioni Booleane]]
- [[#Variabili Booleane]] 
- [[Leggi Booleane]] + [[Legge de consenso(algebra di Boole)|Legge del consenso]]
- [[Operatori Booleani e Porte Logiche]]
- [[#Forma Pos e Sop e dualità di una funzione]]

**Espressioni Booleane:**
- [[Tabelle di verità, Maxtermini e Mintermini]]
- [[Forma normale e canonica di una funzione booleana]]
- [[Uguaglianza tra funzioni booleane]] (da fare)

**Circuiti Logici:**
- [[Mappe di Karnaugh]]
- [[Circuito ed espressione minimale]]
- [[Procedimento di sintesi e analisi]] (aggiungere esempio)
- [[Funzioni non completamente specificate]] (da fare)

---
## Funzioni Booleane
Una **Funzione** o **Equazione booleana** è una combinazione di *variabili* e operatori *booleani* che ritorna una costante *T* o *F*

Le funzioni booleane sono caratterizzate da una o più *variabile di ingresso* e una *variabile di uscita*.

**oss:**
- *Variabili di ingresso:* sono dette **indipendenti**, cioè possono assumere liberamente qualsiasi valore.
- *Variabile di uscita:* è detta **dipendente**, cioè una volta stabilito il valore assunto dalle variabili di ingresso, è obbligata ad assumere un valore.

---
## Variabili Booleane
Le variabili booleane sono lettere che possono assumere due valori *vero*(1) o *falso* (0)

Per convenzione si rappresentano come: 
-  *Vero* = 1 
-  *Falso* = 0

---
## Forma Pos e Sop e dualità di una funzione
**POS (product of sums):** 
- Per forma pos si intende una funzione booleana scritta come prodotti di somme
- Ovvero termini prodotto uniti da somme logiche  

**SOP (sum of products):** 
- Per forma sop si intende una funzione booleana scritta come somma di prodotti
- Ovvero termini somma uniti da prodotti logici logiche  

**Conversione:** per passare dalla forma sop a pos e vice versa basta applicare la legge di demorgan

![[IMG_D4B2236F4378-1.jpeg]]

**Dualità di una funzione booleana**
- Un espressione booleana *E1* è la duale di una espressione *E2* se 
	- Differisce per gli operatori (and e or sono scambiati)
	- Il valore delle costanti (0 e 1 sono scambiati)

- Passare all'espressione duale di un'identità può facilitare la verifica dell'identità
---