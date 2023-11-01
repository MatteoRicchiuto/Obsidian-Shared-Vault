Status: #NotComplete
Academic Year: 2022-2023
Class: [[Logica e Reti Logiche (Class)]], [[3. MOCS/Uni MOC/Uni_Classes/Matematica Discreta (class)]]
Created: Jul 05, 2023
Type: #Uni/Notes

---
# Info



---
# Indice
- [[#Proposizione]]
- [[#Lettere proposizionali]]
- [[#Costanti]]
- [[#Formula ben formata (definizione)]]
- [[#Interpretazioni]]
- [[#Tautologie, contraddizioni, contingenze]]
 
- [[Connettivi logici]]
- [[Leggi Logiche]]

- [[Metodo dei Tableaux nella logica proposizionale]]

- [[Ricavare formula logica da tabella di verità]] <--

- [[Sistemi Assiomatici (Hilbert systems)]] <--

Extra: [[Notazione polacca]]

---
## Proposizione
Una **proposizione semplice** (o atomica) è un’affermazione che: 
-  non dipende da variabili
-  può essere vera o falsa
-  viene formalizzata da un simbolo enunciativo

*Esempi:* 
- Ogni triangolo si può inscrivere in un cerchio vera 
- Roma è in Francia falsa

Una **proposizione composta** può essere:
-  sempre vera
-  sempre falsa
-  vera o falsa in funzione dei componenti

---
## Lettere proposizionali
Chiamiamo *lettere proposizionali* i simboli con p, q, r, . . .  con i quali indichiamo le variabili Booleane, ossia variabili che possono assumere valore True o False 

---
## Costanti
Esistono altre 2 lettere proposizionali `t` e `f` che indicano rispettivamente le variabili Booleane T e F

**Oss:**
- p ∧ f è equivalente a f mentre p ∧ t è equivalente a p 
- p ∨ f è equivalente a p mentre p ∨ t è equivalente a t 
- f ∧ t è equivalente a f mentre f ∨ t è equivalente a t

---
## Formula ben formata (definizione)
- Una **formula** è una sequenza di variabili e connettivi
- Una **formula ben formata** rispetta queste regole:
	1. Ogni *variabile* è una formula
	2. Se *x* è una formula allora *¬x* è una formula
	3. Se *x* e *y* sono formule allora *x* **\*** *y* sono una formula ben formata
		-  dove **\*** è un [[Connettivi logici|connettivo logico]]
	4. Nient’altro è una formula ben formata
	
---
## Interpretazioni
*Definizione:* 
- Data una formula, chiamiamo interpretazione della formula un’assegnazione di verità alle sue variabili 

**oss:** in una tabella di verità, ogni riga rappresenta una diversa interpretazione

- Data una formula `P` ed una interpretazione `τ` di `P`,
- `P` o è T (vera) o è F (falsa) nell’interpretazione τ. 
*Esempio:*
La formula (p ∨ q) ∧ ¬r
- è F (falsa) nell’interpretazione (p, q, r) = ( T , F , T)
- è T nell’interpretazione (p, q, r) = ( T , F , F )

---
## Tautologie, contraddizioni, contingenze
- *Tautologie:* formule che sono T (vere) in ogni interpretazione 
- *Contraddizioni:* formule che sono F (false) in ogni interpretazione
- *contingenze:* formule che sono T in alcune interpretazioni e F in altre

---