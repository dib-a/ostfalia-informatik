---
tags:
  - 1-Semester
  - DS-Diskrete-Strukturen
  - Aussagenlogik
  - Logische-Operatoren
share: "true"
---
# Info
- sprachliche Beschreibung: "Wenn..., dann... (aber vielleicht auch sonst)"
- ist nur dann falsch, wenn A wahr und B falsch ist
- kann man auch schreiben als:
	- $(A \rightarrow B) \Leftrightarrow \lnot A \lor B$
	- $(A \rightarrow B) \Leftrightarrow \lnot B \rightarrow \lnot A$

# Wahrheitstabelle
|     $A$      |     $B$      | $A \rightarrow B$  |
|:------------:|:------------:|:------------:|
| $\mathbb{0}$ | $\mathbb{0}$ | $\mathbb{1}$ |
| $\mathbb{0}$ | $\mathbb{1}$ | $\mathbb{1}$ |
| $\mathbb{1}$ | $\mathbb{0}$ | $\mathbb{0}$ |
| $\mathbb{1}$ | $\mathbb{1}$ | $\mathbb{1}$ |

# [Negation](./Negation.md#) der Subjunktion
- die zweite Aussage wird negiert
- die Verknüpfung wird zu einer Konjunktion
$$\begin{align}
\lnot (A \rightarrow B) &\Leftrightarrow A \land \lnot B\\
\end{align}$$

# Subjunktion anders herum
$A \leftarrow B$:
- sprachliche Beschreibung: 
	- Nur wenn ... dann ... (aber vielleicht auch nicht)
	- Vorausgesetzt ... dann ...


# Modellierung
## Schlüsselwörter
$A \rightarrow B$ 
- auch
- wenn, dann
- impliziert

$A \leftarrow B$ 
- nur wenn, dann
- vorausgesetzt
