---
tags:
  - 1-Semester
  - DS-Diskrete-Strukturen
  - Aussagenlogik
  - Logische-Operatoren
share: "true"
---
# Info
- sprachliche Beschreibung: "entweder...oder..."
- ist genau dann wahr, wenn A und B verschiedene Wahrheitswerte haben
- weitere Bezeichnung: 
	- ausschließende [Disjunktion](./Disjunktion.md#)
	- in der Informatik meist als XOR bezeichnet

# Wahrheitstabelle
|     $A$      |     $B$      | $A \not\leftrightarrow B$  |
|:------------:|:------------:|:------------:|
| $\mathbb{0}$ | $\mathbb{0}$ | $\mathbb{0}$ |
| $\mathbb{0}$ | $\mathbb{1}$ | $\mathbb{1}$ |
| $\mathbb{1}$ | $\mathbb{0}$ | $\mathbb{1}$ |
| $\mathbb{1}$ | $\mathbb{1}$ | $\mathbb{0}$ |

# [Negation](./Negation.md#) der Alternation
- der Operator wird negiert
$$\lnot (A \not\leftrightarrow B) \Leftrightarrow A \leftrightarrow B$$
