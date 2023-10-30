---
Created: 2023-10-20
Type: Uni Note
Class:
  - "[[Calcolo Differenziale (class)]]"
Academic Year: 2023/2024
Related: 
Completed: false
---
---
## Index
1. [[]]

[[Successioni Reali]]
[[Successioni Monotone]]

---
## Operazioni tra successioni 

**Teorema:** 
$$ \begin{align}
&se\ \  a_{n}\to L,\ b_{n}\to M \ allora:\\ \\

&\ \ \ \ 1.  \ \ \ a_{n}\pm b_{n} \to L \pm M \\
&\ \ \ \ 2.  \ \ \ a_{n} \cdot b_{n} \to L \cdot M \\
&\ \ \ \ 3.  \ \ \ \frac{a_{n}}{b_{n}}\to \frac{L}{M} \ \ \ \ \  se \ M \not=0
\end{align}$$
**Casi operazioni e forme indeterminate:** leggi: [[Forme Indeterminate dei Limiti]]
*Teorema 1:*
$$\begin{align}
 & se\ a_{n}\to N, \ \ b_{n}\to + \infty:  \\ \\

&\ \ \ \ -  \ \ \ a_{n}+ b_{n} \to +\infty \\
&\ \ \ \ -  \ \ \ a_{n}- b_{n} \to +\infty \\ 
&\ \ \ \ -  \ \ \ a_{n}\cdot b_{n} \to 
\begin{cases}
   +\infty &\text{if } L>0 \\
    \textcolor{orange}{\text{f.i.}}  &\text{if } L=0 \\
   -\infty &\text{if } L<0 \\
\end{cases} \\

\end{align}$$
*Teorema 2:*
$$\begin{align}
 & se\ a_{n}\to +\infty, \ \ b_{n}\to + \infty:  \\ \\

&\ \ \ \ -  \ \ \ a_{n}+ b_{n} \to +\infty \\
&\ \ \ \ -  \ \ \ a_{n}\cdot b_{n} \to +\infty

\end{align}$$
*Teorema 3:* 
$$\begin{align}
 & se\ a_{n}\to +\infty, \ \ b_{n}\to - \infty:  \\ \\

&\ \ \ \ -  \ \ \ a_{n}+ b_{n} \to +\infty \\
&\ \ \ \ -  \ \ \ a_{n}\cdot b_{n} \to +\infty

\end{align}$$
*oss:* $$a_{n}=\frac{(-1)^n}{n+1}\to 0 \textcolor{orange}{\ \ perche?\ (leggi\ teo.4)}$$
*Teorema 4:*
$$\begin{align}


& Se\ \ a_{n} \ è \ limitata\ e \ b_{n}\to 0\ \ allora:  \\
& \ \ \ \ \ \ \ \ \ \ \ -\ a_{n}\cdot b_{n} \to 0


\end{align} $$
*Teorema 5:*
$$\begin{align}
& Se\ a_{n}\to +\infty\ \ e \ \ b_{n}\geq a_{n}\implies b_{n}\to +\infty \\
& Se\ a_{n}\to -\infty\ \ e \ \ b_{n}\leq a_{n}\implies b_{n}\to -\infty \\ 
\end{align}$$

![[Teorema del Confronto (carabinieri)]]

**All'esame dai spiegazioni del tipo:**
- Limite tende la zero perché il grado del polinomio al denominatore è superiore rispetto al grado del polinomio al numeratore
