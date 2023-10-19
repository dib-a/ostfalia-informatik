---
tags:
  - 1-Semester
  - DS-Diskrete-Strukturen
  - Aussagenlogik
  - Tautologien
share: "true"
---
Aussageformen bzw. logische Ausdrücke, die unabhängig von der Belegung der Variablen immer
- wahr sind, heißen Tautologien $\mathcal{T}$

|     $A$      |     $\lnot A$      |  $A \lor \lnot A$  |
|:------------:|:------------:|:------------:|
| $\mathbb{0}$ | $\mathbb{1}$ | $\mathbb{1}$ |
| $\mathbb{1}$ | $\mathbb{0}$ | $\mathbb{1}$ |

- falsch sind, heißen **Kontradiktionen**

|     $A$      |     $\lnot A$      |  $A \land \lnot A$  |
|:------------:|:------------:|:------------:|
| $\mathbb{0}$ | $\mathbb{1}$ | $\mathbb{0}$ |
| $\mathbb{1}$ | $\mathbb{0}$ | $\mathbb{0}$ |

Wenn die Tautologie eine
- [Bijunktion](../Logische%20Operatoren/Bijunktion.md#) ist, die immer wahr ist
	- wird $\leftrightarrow$ zu $\Leftrightarrow$
	- heißt [Äquivalenz](./%C3%84quivalenz.md#)
 
|     $A$      |     $B$      |  $A \lor B$  | $A \land (A \lor B)$ | $A \land (A \lor B) \leftrightarrow A$ |
|:------------:|:------------:|:------------:|:--------------------:|:--------------------------------------:|
| $\mathbb{0}$ | $\mathbb{0}$ | $\mathbb{0}$ |     $\mathbb{0}$     |              $\mathbb{1}$              |
| $\mathbb{0}$ | $\mathbb{1}$ | $\mathbb{1}$ |     $\mathbb{0}$     |              $\mathbb{1}$              |
| $\mathbb{1}$ | $\mathbb{0}$ | $\mathbb{1}$ |     $\mathbb{1}$     |              $\mathbb{1}$              |
| $\mathbb{1}$ | $\mathbb{1}$ | $\mathbb{1}$ |     $\mathbb{1}$     |              $\mathbb{1}$              |

Hier gilt also $A \land (A \lor B) \Leftrightarrow A$

- [Subjunktion](../Logische%20Operatoren/Subjunktion.md#) ist, die immer wahr ist
	- wird $\rightarrow$ zu $\Rightarrow$
	- heißt [Implikation](./Implikation.md#)
 
|     $A$      |     $B$      | $A \land B$  |  $A \lor B$  | $(A \land B) \rightarrow (A \lor B)$ |
|:------------:|:------------:|:------------:|:------------:|:------------------------------------:|
| $\mathbb{0}$ | $\mathbb{0}$ | $\mathbb{0}$ | $\mathbb{0}$ |             $\mathbb{1}$             |
| $\mathbb{0}$ | $\mathbb{1}$ | $\mathbb{0}$ | $\mathbb{1}$ |             $\mathbb{1}$             |
| $\mathbb{1}$ | $\mathbb{0}$ | $\mathbb{0}$ | $\mathbb{1}$ |             $\mathbb{1}$             |
| $\mathbb{1}$ | $\mathbb{1}$ | $\mathbb{1}$ | $\mathbb{1}$ |             $\mathbb{1}$             |

Hier gilt also $(A \land B) \Rightarrow (A \lor B)$


| Bezeichnung     | Symbol                | Gesprochen                                     |
| --------------- | --------------------- | ---------------------------------------------- |
| [Implikation](./Implikation.md#) | $A \Rightarrow$ B     | A daraus folgt B                               |
| [Äquivalenz](./%C3%84quivalenz.md#)  | $A \Leftrightarrow B$ | A und B haben immer den gleichen Wahrheitswert |

## Präzedenz (Bindungsstärke)

| Priorität |         1         |       2       |         3         | 4      | 5                     | 6       |    7    | 8                  | 9   | 10      |
|:---------:|:-----------------:|:-------------:|:-----------------:|:------:|:---------------------:|:-------:|:-------:|:------------------:|:---:|:-------:|
|           | $\Leftrightarrow$ | $\rightarrow$ | $\leftrightarrow$ | $\lor$ | $\not\leftrightarrow$ | $\land$ | $\lnot$ | $=\not =  < > \leq \geq$ | $+$ | $\cdot$ |

- d.h man bearbeitet einen Ausdruck, indem man die Operatoren von rechts nach links abarbeitet
