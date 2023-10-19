---
tags:
  - TGI-Technische-Grundlagen-der-Informatik
  - Stellenwertsysteme
share: "true"
---
# Grundlagen des Dezimalsystems

## System

Das Dualsystem verwendet 10 Ziffern: $\{0,1,2,3,4,5,6,7,8,9\}$

Berechnung der Anzahl der möglichen Kombinationen

$$\begin{align*}
    10^N &= \text{Anzahl der möglichen Kombinationen}\\
\end{align*}$$

$N:$ Anzahl der Bits

### Beispiel

$$\begin{align*}
N = 4 &: &10^4 &= 10\ 000\\
N = 8 &: &10^8 &= 100\ 000\ 000
\end{align*}$$

Beispiel mit der Zahl: $1938_{10}$

| $10^3$ | $10^2$ | $10^1$ | $10^0$ |
| ------ | ------ | ------ | ------ |
| 1      | 9      | 3      | 8      |

---

# Umwandlung in andere Zahlensysteme

## Umwandlung von Dezimal in Binär

Um eine dezimale Zahl in eine binäre Zahl umzurechnen, verwenden Sie die folgenden Schritte:

1. Teile die Dezimalzahl durch 2.
2. Notiere den Rest (0 oder 1).
3. Teile das Ergebnis erneut durch 2 und notieren Sie den neuen Rest.
4. Wiederhole diese Schritte, bis das Ergebnis 0 ist.
5. Die Binärzahl wird von unten nach oben gelesen, beginnend mit dem letzten Rest.

### Beispiel

Für die Zahl $150_{10}$

| Zahl | :   | Basis | =   | Ergebnis | Rest |
|:----:|:---:|:-----:|:---:|:--------:|:----:|
| 150  | :   | 2     | =   | 75       | 0    |
| 75   | :   | 2     | =   | 37       | 1    |
| 37   | :   | 2     | =   | 18       | 1    |
| 18   | :   | 2     | =   | 9        | 0    |
| 9    | :   | 2     | =   | 4        | 1    |
| 4    | :   | 2     | =   | 2        | 0    |
| 2    | :   | 2     | =   | 1        | 0    |
| 1    | :   | 2     | =   | 0        | 1    |

$$\begin{align*}
	150_{10} = 1001\ 0110_2
\end{align*}$$

## Umwandlung von Dezimal in Hexadezimal

Die Umrechnung verläuft nach demselben Prinzip wie die [Umwandlung von Dezimal in Binär](Dezimalsystem.md#umwandlung-von-dezimal-in-binar)

Die Umrechnung verläuft nach demselben Prinzip wie die 

### Beispiel

Für die Zahl $150_{10}$

| Zahl | :   | Basis | =   | Ergebnis | Rest |
|:----:|:---:|:-----:|:---:|:--------:|:----:|
| 150  | :   |  16   | =   | 9        | 6    |
|  9   | :   |  16   | =   | 0        | 9    |

$$\begin{align*}
	150_{10} = 96_{16}
\end{align*}$$

## Umwandlung von Dezimal in Oktal

Die Umrechnung verläuft nach demselben Prinzip wie die [Umwandlung von Dezimal in Binär](Dezimalsystem.md#umwandlung-von-dezimal-in-binar)

### Beispiel

Für die Zahl $150_{10}$

| Zahl | :   | Basis | =   | Ergebnis | Rest |
|:----:|:---:|:-----:|:---:|:--------:|:----:|
| 150  | :   |   8   | =   | 18       | 6    |
|  18  | :   |   8   | =   |  2       | 2    |
|   2  | :   |   8   | =   |  0       | 2    |

$$\begin{align*}
	150_{10} = 226_8
\end{align*}$$

