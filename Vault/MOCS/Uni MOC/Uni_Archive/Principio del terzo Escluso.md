Class: [[Logica e Reti Logiche (Class)]]
Status: #Complete
Created: June 26, 2023
Academic Year: 2022-2023
Class: [[Logica e Reti Logiche (Class)]]
Macro argomento: [[Teoria degli insiemi]]
Type: #Uni/Notes

---
## Info:

- È uno dei principi fondamentali della logica
- Su di esso di basano le dimostrazioni per assurdo

---
## Enunciato:
 *Il principio del terzo escluso stabilisce che una proposizione e la sua negazione hanno valore di verità opposto*, cioè se abbiamo una situazione che prospetta due vie, di cui una è negazione dell'altra, allora una è vera e l'altra è falsa e non esiste una terza soluzione.

 **In altre parole:** Un affermazione o è vera o la sua negata è vera

**oss:** un affermazione che non rispetta il [[Principio del terzo Escluso]] e il [[Principio di non contraddizione]] si dice [[Paradosso logico]]

---
## Connettivi Logici
Il principio del terzo escluso afferma che:
$$ 
\begin{align*}
& - se ~~ P ~~ è ~~ vera~~ allora ~~\urcorner P ~~ è ~~falsa\\
& - se ~~ P ~~ è ~~ falsa~~ allora ~~\urcorner P ~~ è ~~vera\\
\end{align*}
$$

Utilizzando connettivi logici:
$$ \vDash (p ~ \vee \neg p )  $$

---
## Equivalenza con [[Principio di non contraddizione]]

Utilizzando demorgan è possibili ottenere la definizione logica del principio del terzo escluso

$$ \begin{align}
& - ~\text{principio di non contraddizione:} \vDash \neg(p ~ \land \neg p )\\
& - ~\text{principio del terzo escluso:} \vDash (p ~ \vee \neg p )\\
\end{align} 
 $$
Utilizzando demorgan: 

$$\neg(p ~ \land \neg p ) \leftrightarrow (p ~ \vee \neg p ) $$
