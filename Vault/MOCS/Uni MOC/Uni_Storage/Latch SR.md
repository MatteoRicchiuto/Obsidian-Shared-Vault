---
Created: 2023-11-06
Type: Uni Note
Class:
  - "[[Progettazione Sistemi Digitali (class)]]"
Academic Year: 2023/2024
Related:
  - "[[Circuiti sequenziali]]"
Completed: true
---
---
## Index
1. [[#Definizione]]
2. [[#Circuito]]
3. [[#Stati nel tempo]]

---

## Definizione
- Il **Latch SR** (latch set and reset) è un circuito [[Circuiti sequenziali|sequenziale]] ed [[Circuiti Sincroni ed Asincroni#Circuiti Asincroni|asincrono]] base utilizzato per la memorizzazione di un bit

- S = set
- R = reset
- y = stato del latch (output)
![[IMG_8EEBDB151A76-1.jpeg|200]]

---
## Circuito

![[IMG_799743DAE625-1.jpeg|600]]

---
## Stati nel tempo
*y(t)* = stato presente
*y(t+1)* = stato futuro

**Formula:** $\textcolor{orange}{y(t+1)}=\overline{r+\overline{(s+y(t))}}$
![[IMG_E2122908CA35-1.jpeg|300]]

**Reset:**
$$
\begin{rcases}
   y(t) = 0 \ or  \ 1\\
   s = 0\\
   r = 1\\
\end{rcases}
\to  \textcolor{orange}{y(t+1)}=0
$$

**Set:**
$$
\begin{rcases}
   y(t) = 0 \ or  \ 1\\
   s = 1\\
   r = 0\\
\end{rcases}
\to  \textcolor{orange}{y(t+1)}=1
$$

**Memorizzazione:**
$$
\begin{rcases}
   y(t) = 0 \ or  \ 1\\
   s = 0\\
   r = 0\\
\end{rcases}
\to \textcolor{orange}{y(t+1)}=

\begin{cases}
   0 &\text{se }\ y(t)=0 \\
   1 &\text{se }\ y(t)=1
\end{cases}

$$

---