---
tags:
  - 1-Semester
  - DS-Diskrete-Strukturen
  - Kollektionen
share: "true"
---
# Merkmale
- Reihenfolge ist nicht relevant
- Mehrfachvorkommen ist nicht relevant

In der Informatik ist [Typ](Typ.md#) übrigens ein gängiges Synonym für Menge.
 
# Gleichheit
- müssen die gleichen Elemente haben
$$\begin{align}
\{1,2,3\} &= \{3,2,1,3\}\\
\{1,2,3\} &\neq \{1,2,4\}
\end{align}$$

# Element
Objekte in einer Menge nennt man Elemente $\mathcal{e}$ 
[Aussageformen](../Aussagenlogik/Aussagen-und-Aussageformen.md#aussageformen) wie "x ist Element der Menge M" werden kürzer geschrieben $$x \in M$$
Beispiel
$$M = \{1, \{ 2,3\}, 4, \{ 4,5\}, 5 \}$$
In diesem Beispiel sind $\{2,3\}$ keine Elemente von M also $\{ 2,3 \} \not\in M$ jedoch eine [Teilmenge](Mengen.md#teilmenge). Die Menge, die die Elemente $\{2,3\}$ enthält, also $\{ \{ 2,3 \} \}$ ist ein Element von M. $\{ \{ 2,3 \} \} \in M$ 

Elemente von Mengen müssen nicht atomar sein
- können auch komplexe Strukturen sein
	- [Tupel](./Tupel.md#)
	- [Mengen](Mengen.md#)

# Teilmenge
Eine Menge A ist eine Teilmenge der Menge B, wenn alle Elemente aus A auch in B enthalten sind $$A \subset B$$

In dem oberen Beispiel ist $\{ 4,5\}$ sowohl ein [Element](Mengen.md#element) als auch eine Teilmenge

# Leere Menge
- ist eine Teilmenge jeder Menge
- ist nur dann ein Element, wenn es explizit genannt wird

# Mengen Konstruktor

So kann man Mengen konstruieren (angeben)

| Klammer auf | Elemente                                         | Kontradiktionsstrich | Bedingung(Filter) [Aussageform](../Aussagenlogik/Aussagen-und-Aussageformen.md#aussagen) | Klammer zu |
| ----------- | ------------------------------------------------ | -------------------- | -------------------------------------------------------------------- | ---------- |
| {           | $n : n \in \mathbb{N}$                           | $addLine$            | $n\ mod\ 2 = 1 \land n \leq 100$                                     | }          |
|             | Ausdruck abhängig von Variable: Variable $\in M$ | $\addline$           | Aussageform abhängig von Variable                                    |            |

## Railway-Diagramme
- bildet einen syntaktisch korrekten Ausdruck
- Regeln
	- vom linken Rand durchlaufen
	- ein gültiger Weg, ist ein Weg, der zum Ende führt
	- immer nur in Pfeilrichtung durchlaufen (Einbahnstraße)

==Diagram einfügen ACHTUNG open source!!!==

