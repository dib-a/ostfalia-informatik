---
tags:
  - DS-Diskrete-Strukturen
  - Aussagenlogik
  - Logische-Operatoren
share: "true"
---
# Info

[Aussagen](../Aussagen-und-Aussagenformen.md#aussagen) sind meist zusammengesetzt 
- d.h sie lassen sich zu Teilaussagen zerlegen
- Zusammensetzung erfolgt durch logische Operatoren

Es gilt:
- A,B sind Aussagen

## Liste von logischen Operatoren

| Bezeichnung     |         Symbol         | Gesprochen                                     |
| --------------- |:----------------------:|:---------------------------------------------- |
| [Negation](./Negation.md#)    |       $\lnot A$        | nicht A                                        |
| [Konjunktion](./Konjunktion.md#) |      $A \land B$       | A und B                                        |
| [Disjunktion](./Disjunktion.md#) |       $A \lor B$       | A oder B                                       |
| [Subjunktion](./Subjunktion.md#) |   $A \rightarrow B$    | Wenn A, dann B                                 |
| [Bijunktion](./Bijunktion.md#)  | $A \leftrightarrow B$  | A genau dann, wenn B                           |
| [Alternation](./Alternation.md#) | $A \nleftrightarrow B$ | entweder A oder B                              |

## Präzedenz (Bindungsstärke)

| Priorität |         1         |       2       |         3         | 4      | 5                     | 6       |    7    | 8                  | 9   | 10      |
|:---------:|:-----------------:|:-------------:|:-----------------:|:------:|:---------------------:|:-------:|:-------:|:------------------:|:---:|:-------:|
|           | $\Leftrightarrow$ | $\rightarrow$ | $\leftrightarrow$ | $\lor$ | $\not\leftrightarrow$ | $\land$ | $\lnot$ | $=\not =  < > \leq \geq$ | $+$ | $\cdot$ |

- d.h man bearbeitet einen Ausdruck, indem man die Operatoren von rechts nach links abarbeitet
