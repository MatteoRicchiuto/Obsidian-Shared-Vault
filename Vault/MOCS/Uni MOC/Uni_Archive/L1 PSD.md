---
Created: 2023-09-25
Type: Uni Note
Academic Year: 2023/2024
Class: "[[Progettazione Sistemi Digitali (class)]]"
Related: 
Completed: 
---
---
## Index
1. [[#Info]]
2. [[#Programma]]
3. [[#Architettura di Von Neumann]]
4. [[#Rappresentazione dell'informazione]]
5. [[#Rappresentazione dell'informazione numerica (Naturali)]]

---
# Info

- Prof Annalisa Massimi
- Email massimi@di.uniroma1.it
- Sito: https://bit.ly/CD2324
- Sito2: https://twiki.di.uniroma1.it/twiki/view/Architetture1/EO/CanaleE_O
- Libro: Reti logiche di Morris Mano Kime, Martin 
- Ricevimento: scrivi email per prenotare
- Esami: 1 compito scritto + orale (solo se passi scritto)

---
# Programma
**Prima parte:**
1. Rappresentazione dell'informazione  
2. Porte logiche e circuiti combinatori
3. Algebra di Boole
4. Moduli standard (Decodificatori, Multiplexer, Rom)

**Seconda parte:**
5. Celle di memorizzazione e registri (flip-flop)
6. Circuiti Sequenziali
7. Automi a stati finiti 
8. Moduli standard (Registi di memorizzazione e contatori)
9. HDL (hardware description language Verilog)

---
# [[Architettura di Von Neumann]]
- Prima architettura a programma memorizzato 

**Struttura:**
- CPU
- Memoria
- I/O (input output)
- Bus (collega le strutture)

**Compiti:**
- Elaborazione (CPU)
- Memorizzazione (Memorie)
- Scambio di informazioni (che avviene attraverso I/O)
- Controllo (che sincronizza tutti i compiti) (svolto da CPU )

---
# Rappresentazione dell'informazione
- Alfabeto di supporto 
- Parole o sequenze finite di simboli dell'alfabeto

Funzione di **codifica** che associa informazioni nell'insieme *I* alle parole nell'insieme *C* detto codice 

$$ f: I \to C$$

Funzione di **decodifica**
$$ g: C \to I$$

>[!warning] OSS: 
> - NI = cardinalità di I
 >- NC = cardinaità di C
> - se NI < NC allora codifica si dice *ridondante* 
> - se NI > NC allora codifica si dice *ambigua* 
> 

**Requisisti di una rappresentazione:**
- *Economicità:* minor numero possibile di caratteri
- *Semplicità* di codifica e decodifica
- *Semplicità di elaborazione*

---
# Rappresentazione dell'informazione numerica (Naturali)

**Più info:** [[Sistemi numerici]]

**[[Sistema di numerazione decimale]]**:
- Base: 10
- Simboli: 0, 1 , 2 ,3 , 4, 5, 6, 7, 8 ,9
- Sistema Posizionale

*oss:* con n cifre posso rappresentare 10^n valori diversi

**[[Sistema di numerazione binario]]**:
- Base: 2
- Simboli: 0, 1
- Sistema Posizionale

*oss:* con n cifre posso rappresentare 2^n valori diversi

**Conversione b2-->b10:**
$$ \sum_{i=0}^{n-1}a_{i}\cdot 2^i$$
$$ \text{dove } a_{i} \text{ è il valore associato al bit }b_{i}$$

Esempio:

|b3|b2|b1|b0|
|---|---|---|---|
|0|1|0|1|
valore associato al bit b0 = 1


>[!warning ]  Cifre necessarie per esprimere un numero n (B10) in binario?
>$$ \log_{2}{n} $$
>

**[[Sistema di numerazione esadecimale]]**:
- Base: 16
- Simboli: 0, 1, 2 ,3 ,4 ,5 ,6, 7, 8 ,9 ,A, B ,C, D, E, F
- Sistema Posizionale

---
