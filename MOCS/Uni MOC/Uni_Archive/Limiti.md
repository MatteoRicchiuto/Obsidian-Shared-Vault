---
Created: 2023-05-19
Type: Uni Note
Class:
  - "[[Analisi (Class)]]"
  - "[[Calcolo Differenziale (class)]]"
Related:
  - "[[Funzioni]]"
  - "[[Successioni Reali]]"
Completed:
---
---
## Indice:
**Basi:**
[[Punto di accumulazione]] (aperti, chiusi)
- [[Limiti#Definizione di limite|Definizione di limite]]
- [[Intorni]]
- [[Asintoti]]
- [[Punti di discontinuità]]
- [[Salti]]
- [[interno e frontiera di un insieme]]

**Proprietà:**
- [[Algebra dei limiti]]
- [[Calcolo dei limiti per sostituzione diretta]] <--
- [[Forme Indeterminate dei Limiti]]

- [[Gerarchia degli infiniti]]
- [[Limiti Notevoli]]
- [[Limiti notevoli di Successioni-->0]]

**Tipi:**
- [[Limiti di Funzioni Polinomiali]]
- [[Limiti di Funzioni Razionali]]
- [[Limiti con Esponenziali e Logaritmi]]
- [[Limite Funzioni Elementari]] <--
- [[Limiti di Funzioni Composte]]

- [[Equivalenze asintotiche]]
- [[o piccolo]]

**Teoremi/Strumenti:**
- [[Teorema ponte]]
- [[Teorema di de L'Hopital]] <-- tutto (studiare prima derivate)
- [[Teorema del Confronto (carabinieri)]] <-- manca dimostrazione
- [[Teorema di Heine-Borel (insiemi compatti)]] (senza dimostrazione)
- [[Limiti con Taylor]] <-- studiare prima derivate

---
## Definizione di limite
- Calcolare il limite di una funzione equivale a determinare cosa accade ai valori della funzione man-mano che ci si avvicina a un certo numero reale, o si va a +∞ o -∞

###### **Definizione Formale di limite che tende a un valore finito:**
$$Sia\ \ f:A\subseteq \mathbb{R} \to \mathbb{R}\ \ \ e \ sia \ \ \ X_{0}\in \mathbb{R} \text{ un punto di accumolazione di A. Si dice che:} $$
$$\begin{align}
& \lim_{ n \to x_{0} } f(x) = L  \\
& \\
& dove \ \ L\in \mathbb{R}
\end{align} $$
$$\begin{align}
& \text{Se, per ogni intorno }\ V(L,\delta)\ \text{ esiste un intorno }\ U(x_{0}, \varepsilon)\ \ t.c: \\
& \\
&x\in U(x_{0}, \varepsilon) \cap A \setminus\{x_{0}\} \implies f(x)\in V(L,\delta)
\end{align}$$
![[Screenshot 2023-05-19 at 15.00.56.png]]


