---
tags:
  - TGI-Technische-Grundlagen-der-Informatik
  - Stellenwertsysteme
share: "true"
---
# Grundlagen des Binärsystems

## System

Das Binärsystem verwendet nur zwei Ziffern: $\{0,1\}$

- **1 Bit**: Die kleinste Einheit im Binärsystem wird als "Bit" bezeichnet und kann entweder den Wert 0 oder 1 haben. Bit steht für "binary digit".
- **1 Nibble**: Ein "Nibble" besteht aus 4 Bits. Ein Nibble kann 16 verschiedene Kombinationen von 0-en und 1-en darstellen.
- **1 Byte**: Ein "Byte" besteht aus 8 Bits und ist eine gebräuchliche Größe in der digitalen Datenverarbeitung. Ein Byte kann 256 verschiedene Kombinationen von 0-en und 1-en darstellen.

Berechnung der Anzahl der möglichen Kombinationen

$$\begin{align*}
    2^N &= \text{Anzahl der möglichen Kombinationen}\\
\end{align*}$$

$N:$ Anzahl der Bits

### Beispiel

$$\begin{align*}
N = 4 &: &2^4 &= 16\\
N = 8 &: &2^8 &= 256
\end{align*}$$

Beispiel mit der Zahl: $0111_2$ 

| $2^3$ | $2^2$ | $2^1$ | $2^0$ |
|:-----:|:-----:|:-----:|:-----:|
|   8   |   4   |   2   |   1   |
|   0   |   1   |   1   |   1   |

---

# Umwandlung in andere Zahlensysteme

## Umwandlung von Binär in Dezimal

Die Umwandlung von binären Zahlen in dezimale Zahlen erfolgt mithilfe einer mathematischen Formel, die die Gewichtung der Binärstellen berücksichtigt.

$$\begin{align}
    z = \sum_{i=0}^{n-1}{a_i\cdot 2^i}
\end{align}$$

$z$ ist die Dezimalzahl<br>
$n$ ist die Anzahl der Binärstellen<br>
$a_i$ ist die Binärziffer an der Stelle i<br>
$2$ ist die Basis für das Binärsystem

### Beispiel
Angenommen, wir haben die binäre Zahl $0111_2$ und möchten sie in eine Dezimalzahl umwandeln:

$$\begin{align}
  z &= (1 \cdot 2^0) + (1 \cdot 2^1)+ (1 \cdot 2^2) + (0 \cdot 2^3)\\ 
  &= 1 + 2 + 4 + 0 \\
  &= 7_{10}\\
\end{align}$$

$$\begin{align}
	0111_2 &= 7_{10}
\end{align}$$

## Umrechnung von Binär in Hexadezimal

> [!NOTE]
> Da 2^4 = 16, können alle 4 Bits (1 Nibble) in eine Hexadezimalziffer übersetzt werden.

### Anleitung
Die Umwandlung von Binär zu Hexadezimal erfolgt in den folgenden Schritten:
 
1. Binärzahl in 4-er Bits (Nibble) aufteilen
2. Alle 4-er Bits separat umrechnen
3. Ergebnisse zusammenführen

### Beispiel

|    Gegeben     | $0111\ 1110_2$ |          |
|:--------------:|:--------------:|:--------:|
|   Aufteilung   |    $0111_2$    | $1110_2$ |
|   Umrechnung   |    $7_{16}$    | $E_{16}$ |
| Zusammenführen |   $7E_{16}$    |          |

$$\begin{align*}
    0111\ 1110_2 = 7E_{16}
\end{align*}$$

## Umrechnung von Binär in Oktal

> [!NOTE]
> Da 2^3 = 8, können alle 3 Bits in eine Oktalziffer umgewandelt werden.

### Anleitung
Die Umwandlung von Binär zu Oktal erfolgt in den folgenden Schritten:
 
1. Binärzahl in 3-er Bits aufteilen
2. Alle 3-er Bits separat umrechnen
3. Ergebnisse zusammenführen

### Beispiel

Für $0111\ 1110_2$

|   Aufteilung   |    $001_2$     | $111_2$ | $110_2$ |
|:--------------:|:--------------:|:-------:|:-------:|
|   Umrechnung   |     $1_8$      |  $7_8$  |  $6_8$  |
| Zusammenführen |    $176_8$     |         |         |

$$\begin{align*}
    0111\ 1110_2 = 176_8
\end{align*}$$

---

# Rechnen

## Binäre Addition

### Anleitung
1. Beginne mit der Addition von rechts nach links, ähnlich wie bei der Addition im Dezimalen.
2. Addiere die Bits von rechts nach links, beginnend mit dem niedrigsten Subtraktion im Bit (dem rechtesten Bit).
3. Führe bei einer Summe von $2_{10}$ ($10_2$) eine Übertragung zum nächsten Bit durch.
4. Schreiben Sie das Ergebnis in Binärform auf.

### Beispiel

$7_{10} + 3_{10}$

$$\begin{align*}
	7_{10} &= 0111_2\\
	3_{10} &= 0011_2
\end{align*}$$

|          |  0  |  1  |  1  |  1  |
|:--------:|:---:|:---:|:---:|:---:|
|    +     |  0  |  0  |  1  |  1  |
| Übertrag |  1  |  1  |  1  |     |
|          |     |     |     |     |
|    =     |  1  |  0  |  1  |  0  |

$$\begin{align*}
    7_{10} + 3_{10} = 0111_2 + 0011_2 = 1010_2 = 10_{10}
\end{align*}$$

## Binäre Subtraktion

### Anleitung
1. Beginne mit der Subtraktion von rechts nach links, ähnlich wie bei der Dezimalsubtraktion.
2. Subtrahiere die Bits von rechts nach links, beginnend mit dem niedrigsten Bit (dem rechtesten Bit).
3. Führe eine Ausleihe zum nächsten Bit durch, wenn das Subtrahieren nicht möglich ist (zum Beispiel bei 0 - 1).
4. Schreibe das Ergebnis in Binärform auf.

### Beispiel

$7_{10} - 3_{10}$

|          |  0  |  1  |  1  |  1  |
|:--------:|:---:|:---:|:---:|:---:|
|    -     |  0  |  0  |  1  |  1  |
| Ausleihe |     |     |     |     |
|          |     |     |     |     |
|    =     |  0  |  1  |  0  |  0  |

$$\begin{align*}
    7_{10} - 3_{10} = 0111_2 - 0011_2 = 0100_2 = 4_{10}
\end{align*}$$

---
# Darstellung ganzer Zahlen

## Vorzeichen-Betragsdarstellung (Sign-Magnitude Representation)

Das erste Bit in der Vorzeichen-Betragsdarstellung gibt das Vorzeichen der Zahl an,

- 0: Die Zahl ist positiv.
- 1: Die Zahl ist negativ.

während die verbleibenden Bits den Betrag repräsentieren.

$-4_{10}$ wird in binärer Darstellung als $1100_2$ dargestellt, wobei das erste Bit das negative Vorzeichen anzeigt. Der Betrag ist $110_2 = 4_{10}$.

### Darstellbarer Bereich
Der darstellbare Bereich in der Vorzeichen-Betragsdarstellung erstreckt sich von:

$$\begin{align*}
    -(2^{N-1}-1)...0...(2^{N-1}-1)
\end{align*}$$

$N:$ Anzahl der Bits

Für 4-Bit Darstellung (N=4) reicht der Bereich von: 

$$\begin{align*}
    -(2^{4-1}-1)&...0...(2^{4-1}-1)\\
    -7&...0... 7
\end{align*}$$

### Nachteile
- doppelte Darstellung von $0_{10}$ ($0000_2$ für "+0" und $1000_2$ für "-0") 
- die Begrenzung des darstellbaren Bereichs

## Einerkomplement

### Schritte zum Einerkomplement
1. Positive Zahl in binär aufschreiben
2. Alle Bits invertieren (negieren). D.h aus 0 wird 1 und aus 1 wird 0

### Beispiel
$-7_{10}$

$$\begin{align*} 
    7_{10} &= 0111_2\\
    -7_{10} &= 1000_2
\end{align*}$$

### Darstellbarer Bereich
Der darstellbare Bereich beim Einerkomplement erstreckt sich von:

$$\begin{align*}
    -(2^{N-1}-1)...0...(2^{N-1}-1)
\end{align*}$$

### Nachteile
- doppelte Darstellung von $0_{10}$ ($0000_2$ für "+0" und $1111_2$ für "-0") 
- die Begrenzung des darstellbaren Bereichs

## Addition im Einerkomplement

### Beispiel

$-7_{10} + 11_{10}$

$$\begin{align*}
    7_{10} &= 0111_2\\
    -7_{10} &= 1000_2\\
    11_{10} &= 1011_2\\
\end{align*}$$

|          |     |  1  |  0  |  0  |  0  |
|:--------:|:---:|:---:|:---:|:---:|:---:|
|    +     |     |  1  |  0  |  1  |  1  |
| Überlauf |  1  |     |     |     |     |
|          |     |     |     |     |     |
|    =     |     |  0  |  0  |  1  |  1  |


> [!WARNING]
> Der Überlauf muss nochmal dazu addiert werden

|          |     |  0  |  0  |  1  |  1  |
|:--------:|:---:|:---:|:---:|:---:|:---:|
|    +     |     |  0  |  0  |  0  |  1  |
| Überlauf |     |     |  1  |  1  |     |
|          |     |     |     |     |     |
|    =     |     |  0  |  1  |  0  |  0  |

$$\begin{align*}
    -7_{10} + 11_{10} = (1000_2 + 1011_2) + 0001_2 = 0100_2 = 4_{10}
\end{align*}$$

## Subtraktion im Einerkomplement

Nutze die Regel: $a - b = a + (-b)$<br>
d.h mach aus einer Subtraktion eine Addition mit einer negativen Zahl

## Zweierkomplement

### Schritte zum Zweierkomplement
1. [Einerkomplement](Binärsystem(Dualsystem).md#einerkomplement) bilden
2. $0001_2$ addieren

### Beispiel
$-7_{10}$

$$\begin{align*} 
    &1.1&\ 7_{10} &= 0111_2\\
    &1.2&\ -7_{10} &= 1000_2\\
    &2.&\ -7_{10} + 0001_2 &= 1001_2
\end{align*}$$

### Darstellbarer Bereich
Der darstellbare Bereich beim Zweierkomplement erstreckt sich von:

$$\begin{align*}
    -(2^{N-1})...0...(2^{N-1}-1)
\end{align*}$$

## Addition im Zweierkomplement

### Beispiel

$-7_{10} + 11_{10}$

$$\begin{align*}
    7_{10} &= 0111_2\\
    -7_{10} &= 1000_2\\
    -7_{10} + 0001_2 &= 1001_2\\
    11_{10} &= 1011_2\\
\end{align*}$$

|          |     |  1  |  0  |  0  |  1  |
|:--------:|:---:|:---:|:---:|:---:|:---:|
|    +     |     |  1  |  0  |  1  |  1  |
| Überlauf |  1  |     |  1  |  1  |     |
|          |     |     |     |     |     |
|    =     |     |  0  |  1  |  0  |  0  |

> [!NOTE]
> Der Überlauf kann ignoriert werden

$$\begin{align*}
    -7_{10} + 11_{10} = 1001_2 + 1011_2 = 0100_2 = 4_{10}
\end{align*}$$

## Subtraktion im Zweierkomplement

Nutze die Regel: $a - b = a + (-b)$<br>
d.h mach aus einer Subtraktion eine Addition mit einer negativen Zahl

$$\begin{align*}
    0111_2 &= 7_{10}
\end{align*}$$
