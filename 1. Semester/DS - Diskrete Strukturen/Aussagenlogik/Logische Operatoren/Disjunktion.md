---
tags:
  - 1-Semester
  - DS-Diskrete-Strukturen
  - Aussagenlogik
  - Logische-Operatoren
share: "true"
---
# Info
- gesprochen "oder auch"
- ist ein binärer Operator
	- wirkt auf zwei Operanden
- ist genau dann wahr, wenn A, B oder beide wahr sind

# Wahrheitstabelle
|     $A$      |     $B$      | $A \lor B$  |
|:------------:|:------------:|:------------:|
| $\mathbb{0}$ | $\mathbb{0}$ | $\mathbb{0}$ |
| $\mathbb{0}$ | $\mathbb{1}$ | $\mathbb{1}$ |
| $\mathbb{1}$ | $\mathbb{0}$ | $\mathbb{1}$ |
| $\mathbb{1}$ | $\mathbb{1}$ | $\mathbb{1}$ |

# [Negation](./Negation.md#) der Disjunktion
- Die Aussagen, die mit der Disjunktion verknüpft sind, werden negiert
- Die Verknüpfung wird zu einer [Konjunktion](./Konjunktion.md#) 
$$\lnot (A \lor B) \Leftrightarrow \lnot A \land \lnot B$$
