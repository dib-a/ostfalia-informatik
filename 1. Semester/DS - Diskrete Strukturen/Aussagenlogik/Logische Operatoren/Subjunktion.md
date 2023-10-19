---
tags:
  - DS-Diskrete-Strukturen
  - Aussagenlogik
  - Logische-Operatoren
share: "true"
---
# Info
- ist nur dann falsch, wenn A wahr und B falsch ist
- sprachliche Beschreibung: "Wenn..., dann... (aber vielleicht auch sonst)"
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

# Negation der Subjunktion
- die zweite Aussage wird negiert
- die Verknüpfung wird zu einer Konjunktion
$$\lnot (A \rightarrow B) \Leftrightarrow A \land \lnot B$$

# Subjunktion anders herum
$A \leftarrow B$:
- sprachliche Beschreibung: 
	- Nur wenn ... dann ...
	- Vorausgesetzt ... dann ...
