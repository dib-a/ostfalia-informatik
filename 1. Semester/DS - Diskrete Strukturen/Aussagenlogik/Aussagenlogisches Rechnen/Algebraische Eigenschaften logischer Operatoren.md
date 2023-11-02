---
tags:
  - 1-Semester
  - DS-Diskrete-Strukturen
  - Aussagenlogik
share: "true"
---
# Gesetze
| Bezeichnung          | Beispiel für $\land$                                | Beispiel für $\lor$                                |
| -------------------- | --------------------------------------------------- | -------------------------------------------------- |
| Kommutativgesetz     | $A \land B = B \land A$                             | $A \lor B = B \lor A$                              |
| Assoziativgesetz     | $(A \land B) \land C = A \land (B \land C)$         | $(A \lor B) \lor C = A \lor (B \lor C)$            |
| Idempotenz           | $A \land A = A$                                     | $A \lor A = A$                                     |
| Distributivgesetz    | $A \land (B \lor C) = (A \land B) \lor (A \land C)$ | $A \lor (B \land C) = (A \lor B) \land (A \lor C)$ |
| Neutralitätsgesetz   | $A \land 1 = A$                                     | $A \lor 0 = A$                                     |
| Exremalgesetz        | $A \land 0 = 0$                                     | $A \lor 1 = 1$                                     |
| De Morgansche Gesetz | $\lnot (A \land B) = \lnot A \lor \lnot B$          | $\lnot (A \lor B) = \lnot A \land \lnot B$         |
| Komplementärgesetz   | $A \land \lnot A = 0$                               | $A \lor \lnot A = 1$                               |
| Dualitätsgestz       | $\lnot 0 = 1$                                       | $\lnot 1 = 0$                                      |
| Absorptionsgesetz    | $A \lor (A \land B) = A$                            | $A \land (A \lor B) = A$                           |
| Doppelte Negation    | $\lnot \lnot A = A$                                 |                                                    |

# Transitiv
Ein binärer logischer Operator heißt transitiv, wenn gilt:

$$
A \bullet B \land B \bullet C \Rightarrow A \bullet C
$$

# Minimalset binärer logischer Operatoren
Alle 16 logische Operatoren lassend sich mit $\lnot, \land$ und $\lor$ ausdrücken