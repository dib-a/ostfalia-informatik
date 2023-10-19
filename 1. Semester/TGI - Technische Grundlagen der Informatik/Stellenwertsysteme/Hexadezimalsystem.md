---
tags:
  - 1-Semester
  - TGI-Technische-Grundlagen-der-Informatik
  - Stellenwertsysteme
share: "true"
---
# Grundlagen des Hexadezimalsystems 

## System

Das Dualsystem verwendet 16 Ziffern: $\{0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F\}$

Berechnung der Anzahl der möglichen Kombinationen

$$\begin{align*}
  16^N &= \text{Anzahl der möglichen Kombinationen}\\
\end{align*}$$

$N:$ Anzahl der Bits

### Beispiel

$$\begin{align*}
N = 4 &: &16^4 &= 65\ 536\\
N = 8 &: &16^8 &= 4\ 294\ 967\ 296
\end{align*}$$

Beispiel mit der Zahl: $19A8_{16}$

| $16^3$ | $16^2$ | $16^1$ | $16^0$ |
| ------ | ------ | ------ | ------ |
| 1      | 9      | A      | 8      |

---

# Umwandlung in andere Zahlensysteme

## Umwandlung von Hexadezimal in Binär

> [!NOTE] Hinweis
> Um eine Hexadezimal Zahl in eine binäre Zahl umzurechnen, kann man verwenden, dass 2^4 = 16 ist.
> D.h mann kann jede Ziffer aus dem Hexadezimalsystem in 4 Bits (1 Nibble) aus dem Binärsystem übersetzen

### Beispiel

Für die Zahl $19A8_{16}$

| 1    | 9    | A    | 8    |
|:----:|:----:|:----:|:----:|
| 0001 | 1001 | 1010 | 1000 |

$$\begin{align*}
	19A8_{16} = 0001\ 1001\ 1010\ 1000_2
\end{align*}$$

## Umwandlung von Hexadezimal in Dezimal

Die Umwandlung von hexadezimalen Zahlen in dezimale Zahlen erfolgt mithilfe einer mathematischen Formel, die die Gewichtung der Hexadezimalstellen berücksichtigt.

Die Umrechnung erfolgt mithilfe der Formel:

$$\begin{align}
  z = \sum_{i=0}^{n-1}{a_i\cdot 16^i}
\end{align}$$

$z$ ist die Dezimalzahl<br>
$n$ ist die Anzahl der Binärstellen<br>
$a_i$ ist die Binärziffer an der Stelle i<br>
$16$ ist die Basis für das Binärsystem

### Beispiel
Angenommen, wir haben die hexadezimale Zahl $19A8_{16}$ und möchten sie in eine Dezimalzahl umwandeln:

$$\begin{align}
  z &= (8 \cdot 16^0) + (10 \cdot 16^1)+ (9 \cdot 16^2) + (1 \cdot 16^3)\\ 
  &= 8 + 160 + 2304 + 4096 \\
  &= 6\ 568_{10}\\
\end{align}$$

$$\begin{align}
	19A8_{16} &= 6\ 568_{10}
\end{align}$$

## Umwandlung von Hexadezimal in Oktal

1. [Umwandlung von Hexadezimal in Binär](Hexadezimalsystem.md#umwandlungvonhexadezimalinbinar)
2. [Umwandlung von Binär in Oktal](Binärsystem-(Dualsystem).md#umrechnung%5Cvon%5Cbinär%5Cin%5Coktal)
