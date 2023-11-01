---
Created: 2023-10-03
Type: Uni Note
Class:
  - "[[Progettazione Sistemi Digitali (class)]]"
Academic Year: 2023/2024
Related:
  - "[[Sistema di numerazione binario]]"
Completed:
---
---
## Indice
1. [[#Definizione]]
2. [[#Standard IEEE754]]
3. [[#Notazione scientifica]]
4. [[#Conversioni]]
5. [[#Bias]]
6. 

---
## Definizione
Ogni numero binario in virgola mobile è composto da una *tripla di valori*:
1. Segno (pos 0, neg 1)
2. Esponente (quanti numeri fanno parte della parte intera)
3. Mantissa (cifre dopo la virgola)

**Vantaggi:**
- Rappresentazione mobile permette di ottimizzare al massimo l’utilizzo dei bit a disposizione, permettendo di utilizzare il miglior rapporto tra precisione della parte intera e della parte decimale in base al numero che dobbiamo rappresentare

**Svantaggi:**
- Conversione meno intuitiva per l'essere umano

---
## Standard IEEE754

**Half precision:** 
- Totale: 16 bit
- Segno: 1 bit
- Esponente: 5
- Mantissa: 10

**Single Precision:**
- Totale: 32 bit
- Segno: 1 bit
- Esponente: 8 bit
- Mantissa: 23 bit

**Double Precision:**
- Totale: 64 bit
- Segno: 1 bit
- Esponente: 11 bit
- Mantissa: 52 bit

---
## Notazione scientifica
Capire la notazione scientifica di un numero in binario è fondamentale per capire il funzionamento della virgola mobile

Lo stesso principio che si utilizza per la notazione scientifica di un numero in base 10 si può utilizzare per un numero in binario ma utilizzando potenze di due

**Esempio:**


---
## Conversioni
**B10 -> B2 Floating Point:**
1. Converto il numero in binario (utilizzando [[Numeri binari con virgola fissa (fixed point)|metodo virgola fissa]])
2. Sposto la virgola, trovando mantissa e l'esponente (forma: 1,*M* \* 2^*e* )
3. Aggiungo bias all'esponente (*k*)
4. Converto esponente in binario
5. Scrivo segno (pos = 0, neg = 1)
![[IMG_F3C704D30BCE-1.jpeg]]

**B2 Floating Point -> B10**
1. Utilizzare formula: $$(-1)^\textcolor{orange}{s}\ \cdot\ (1,\textcolor{orange}{M})\ \cdot\ 2^{\textcolor{orange}{e}-k} $$
2. Convertire risultato in decimale usando metodo [[Numeri binari con virgola fissa (fixed point)|fixed point b2->b10]]

![[IMG_426888D244DD-1.jpeg]]

*oss:*
- s = segno
- M = mantissa
- e = esponente
- k = bias

**Conversione numeri periodici:**
Quando si ha un numero binario periodico (virgola fissa) per rappresentarlo in virgola mobile bisogna avere degli accorgimenti

Quando si scrive la mantissa e non si anno abbastanza cifre per completarla invece di estenderla con degli zeri va estesa ricopiando la parte iniziale della mantissa
![[IMG_5D6532D13598-1.jpeg]]

---
## Bias
Il bias è un valore che dipende dalla lunghezza di rappresentazione che utilizziamo ed è utilizza to per correggere l'errore di bias negli esponenti 

- Half precision: 
- Single Precision: 127
- Double Precision:

**Cos'è e come si calcola il bias:**
$$2^{\textcolor{orange}{E}-1}-1$$
Dove *E* è il numero di bit dell'esponente

---
## Operazioni
**Addizione e sottrazione:**
1. Normalizziamo i due numeri (ovvero stesso esponente)
2. Mantissa più grande sopra, più piccola sotto
3. Se segno concorde somma se discorde sottrazione 
4. Segno del risultato è segno del più grande

**Prodotto e divisione:**
1. Sommare / sottrarre gli esponenti 
2.  Moltiplicazioni / dividere le mantisse
3. Segno: 
	- Negativo (operandi discordi)
	- Positivo (operandi concordi)
	- Il risultato potrebbe essere normalizzato (ovvero riportare alla rappresentazione standard (1,*M*) aggiustando esponente)

---
