Status: #Complete
Academic Year: 2022-2023
Class: [[Analisi (Class)]], 
Created: May 26, 2023
Type: #Uni/Notes
Related: [[Limiti]]

---
# Definizione

$$\begin{align}
& - \ \ \text{Siano f(x) e g(x) due funzioni definite in un introno di x0,} \\ 
& \ \ \ \ \ \  \ \text{dove }x_{0} \in \mathbb{R} \\ \\
& - \ \ se \ \lim_{ x \to x_{0} }\frac{f(x)}{g(x)}=0\ \ \ \ allora: \\ \\
&- \ \ f(x) = o(g(x))\ \ per\ \ x\to x_{0}
  
\end{align} $$

**Intuitivamente:**
- *f(x) è un o piccolo di di g(x)*  per x-->x0 è equivalente a dire che *f(x) è infinitamente più piccola, rispetto a g(x)*, quando x-->x0


---
# Proprietà:
$$
\begin{align} 
& 1.\ \ o(x) \pm o(x) = o(x)  \\   \\
& \ \ \ \ \ \ \ \ \ \ \ \ \textcolor{orange}{oss:}\ o(x^n)\pm o(x^n)=o(x^n)\\ \\ 
& 2.\ \ o(x^n) \cdot 0(x^m)=0(x^{n+m})\\ \\
& \ \ \ \ \ \ \ \ \ \ \ \ \textcolor{orange}{oss:}\ x^n\cdot o(x^m)=o(x^{n+m})\\ \\ 
& 3.\ \ x^n=o(x^m) \ \ \ se \ x\to 0 \ \ e \ \ n>m  \\ \\
& 4.\ \ o(x^n)\pm o(x^m) = o(n^n) \ \ \ se \ x\to 0 \ \ e \ \ n<m  \\
\end{align}
$$
---
# Esempi:
![[Screenshot 2023-05-26 at 11.48.27.png]]

---