---
tags:
  - DS-Diskrete-Strukturen
  - Aussagenlogik
  - Logische-Operatoren
share: "true"
---
# Info
- ist genau dann wahr, wenn A und B verschiedene Wahrheitswerte haben
- sprachliche Beschreibung: "entweder...oder..."
- in der Informatik meist als xor bezeichnet
- weitere Bezeichnung: ausschließende [Disjunktion](./Disjunktion.md#)

### Wahrheitstabelle
|     $A$      |     $B$      | $A \not\leftrightarrow B$  |
|:------------:|:------------:|:------------:|
| $\mathbb{0}$ | $\mathbb{0}$ | $\mathbb{0}$ |
| $\mathbb{0}$ | $\mathbb{1}$ | $\mathbb{1}$ |
| $\mathbb{1}$ | $\mathbb{0}$ | $\mathbb{1}$ |
| $\mathbb{1}$ | $\mathbb{1}$ | $\mathbb{0}$ |

### Negation der Alternation
- der Operator wird negiert
$$\lnot (A \not\leftrightarrow B) \Leftrightarrow A \leftrightarrow B$$
