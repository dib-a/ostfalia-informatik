---
tags:
  - TGI-Technische-Grundlagen-der-Informatik
  - Stellenwertsysteme
share: "true"
---
# Grundlagen des Oktalsystems 

## System

Das Dualsystem verwendet 8 Ziffern: $\{0,1,2,3,4,5,6,7\}$

Berechnung der Anzahl der möglichen Kombinationen

$$\begin{align*}
  8^N &= \text{Anzahl der möglichen Kombinationen}\\
\end{align*}$$

$N:$ Anzahl der Bits

### Beispiel

$$\begin{align*}
N = 4 &: &8^4 &= 4\ 096\\
N = 8 &: &8^8 &= 16\ 777\ 216
\end{align*}$$

Beispiel mit der Zahl: $3742_{8}$

| $8^3$ | $8^2$ | $8^1$ | $8^0$ |
| ------ | ------ | ------ | ------ |
| 3      | 7      | 4      | 2      |

---

# Umwandlung in andere Zahlensysteme

## Umwandlung von Oktal in Binär

> [!NOTE]
> Da 2^3 = 8, kann jede Oktalziffer in 3 binäre Ziffern umgewandelt werden.

### Beispiel

Für die Zahl $3742_{8}$

|  3  |  7  |  4  |  2  |
|:---:|:---:|:---:|:---:|
| 011 | 111 | 100 | 010 |

$$\begin{align*}
	3742_{8} = 0111\ 1110\ 0010_2
\end{align*}$$

## Umwandlung von Oktal in Dezimal

Die Umwandlung von oktalen Zahlen in dezimale Zahlen erfolgt mithilfe einer mathematischen Formel, die die Gewichtung der Oktalstellen berücksichtigt.

Die Umrechnung erfolgt mithilfe der Formel:

$$\begin{align}
  z = \sum_{i=0}^{n-1}{a_i\cdot 8^i}
\end{align}$$

$z$ ist die Dezimalzahl<br>
$n$ ist die Anzahl der Binärstellen<br>
$a_i$ ist die Binärziffer an der Stelle i<br>
$8$ ist die Basis für das Binärsystem

### Beispiel
Angenommen, wir haben die oktale Zahl $3742_{8}$ und möchten sie in eine Dezimalzahl umwandeln:

$$\begin{align}
  z &= (2 \cdot 8^0) + (4 \cdot 8^1)+ (7 \cdot 8^2) + (3 \cdot 8^3)\\ 
  &= 2 + 32 + 448 + 1536\\
  &= 2\ 018_{10}\\
\end{align}$$

$$\begin{align}
	3742_{8} &= 2\ 018_{10}
\end{align}$$

## Umwandlung von Oktal in Hexadezimal

1. [Umwandlung von Oktal in Binär](Oktalsystem.md#umwandlung-von-oktal-in-binar)
2. [Umwandlung von Binär in Hexadezimal](./Binärsystem(Dualsystem).md#umrechnung-von-binar-in-hexadezimal) 
