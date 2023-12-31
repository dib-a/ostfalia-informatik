---
tags:
  - 1-Semester
  - DS-Diskrete-Strukturen
  - Aussagenlogik
  - Logische-Operatoren
share: "true"
---
# Info
- sprachliche Beschreibung: "und"
- ist ein binärer Operator
	- wirkt auf zwei Operanden
- ist genau dann wahr, wenn A und B wahr sind

# Wahrheitstabelle
|     $A$      |     $B$      | $A \land B$  |
|:------------:|:------------:|:------------:|
| $\mathbb{0}$ | $\mathbb{0}$ | $\mathbb{0}$ |
| $\mathbb{0}$ | $\mathbb{1}$ | $\mathbb{0}$ |
| $\mathbb{1}$ | $\mathbb{0}$ | $\mathbb{0}$ |
| $\mathbb{1}$ | $\mathbb{1}$ | $\mathbb{1}$ |

# [Negation](./Negation.md#) der Konjunktion
- Die Aussagen, die mit der Konjunktion verknüpft sind, werden negiert
- Die Verknüpfung wird zu einer [Disjunktion](./Disjunktion.md#)
$$\lnot (A \land B) \Leftrightarrow \lnot A \lor \lnot B$$
