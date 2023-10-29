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

**Für die folgenden Beispiele gilt:** 

![mengen.png](./images/mengen.png#)

blau: Menge A
gelb: Menge B
grün: Verknüpfung
# Teilmenge
Eine Menge A ist eine Teilmenge der Menge B, wenn alle Elemente aus A auch in B enthalten sind $$A \subseteq B$$

![teilmenge.png](./images/teilmenge.png#)

In dem oberen Beispiel ist $\{ 4,5\}$ sowohl ein [Element](Mengen.md#element) als auch eine Teilmenge

# Leere Menge
- geschrieben: $\varnothing$ oder { }
- ist eine Teilmenge jeder Menge
- ist nur dann ein Element, wenn es explizit genannt wird


> [!Warning] Leere Menge
> Die Leere Menge ist eine Teilmenge jeder Menge. Sie ist aber nur dann ein Element der Menge, wenn sie explizit angegeben wird

# Mengen Konstruktor

So kann man Mengen konstruieren (angeben)

| Klammer auf |                     Elemente                     | Kontradiktionsstrich | Bedingung(Filter) [Aussageform](../Aussagenlogik/Aussagen-und-Aussageformen.md#aussagen) | Klammer zu |
|:-----------:|:------------------------------------------------:|:--------------------:|:--------------------------------------------------------------------:|:----------:|
|      {      |              $n : n \in \mathbb{N}$              |          \|          |                   $n\ mod\ 2 = 1 \land n \leq 100$                   |     }      |
|             | Ausdruck abhängig von Variable: Variable $\in M$ |          \|          |                  Aussageform abhängig von Variable                   |            |

## Railway-Diagramme
- bildet einen syntaktisch korrekten Ausdruck
- Regeln
	- vom linken Rand durchlaufen
	- ein gültiger Weg, ist ein Weg, der zum Ende führt
	- immer nur in Pfeilrichtung durchlaufen (Einbahnstraße)

==Diagram einfügen ACHTUNG open source!!!== --- fragen ob das aus dem Skript übernommen werden darf

# Mächtigkeit
die Anzahl der Elemente einer Menge wird Mächtigkeit ($|\{...\} |$) genannt
$$\begin{align*}
	|\{ 1,2,3 \}| = 3
\end{align*}$$
# Operationen auf Mengen

## Vereinigung

$$\begin{align*}
	A \cup B = \{ x:x \in \mathbb{U} \mid x \in A \lor x \in B \}
\end{align*}$$

![vereinigung.png](./images/vereinigung.png#)

## Schnitt

$$\begin{align*}
	A \cap B = \{ x:x \in \mathbb{U} \mid x \in A \land x \in B \}
\end{align*}$$

![schnittmenge.png](./images/schnittmenge.png#)

Wenn der Schnitt zweier Mengen leer ist nennt man die Mengen disjunkt

## Differenz

$$\begin{align*}
	A \setminus B = \{ x:x \in \mathbb{U} \mid x \in A \land x \not\in B \}
\end{align*}$$

![differenz.png](./images/differenz.png#)

## Komplement

$$\begin{align*}
	\overline A = \{ x:x \in \mathbb{U} \mid x \not\in A \}
\end{align*}$$

![komplement.png](./images/komplement.png#)

# Algebraische Eigenschaften

| Bezeichnung                | Beispiel für $\cup$                                  | Beispiel für $\cap$                                  |
| -------------------------- | ---------------------------------------------------- | ---------------------------------------------------- |
| neutrales Element          | $A \cup \varnothing = A$                             | $A \cap \varnothing = A$                             |
| Komplementarität           | $A \cup \overline A = \mathbb{U}$                    | $A \cap \overline A = \varnothing$                   |
| Assoziativität             | $A \cup (B \cup C) = (A \cup B) \cup C$              | $A \cap (B \cap C) = (A \cap B) \cap C$              |
| Kommutativität             | $A \cup B = B \cup A$                                | $A \cap B = B \cap A$                                |
| Distributivität            | $A \cup (B \cap C) = (A \cup B) \cap (A \cup C)$     | $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$     |
| de Morgan'sche Regeln      | $\overline{A \cup B} = \overline A \cap \overline B$ | $\overline{A \cap B} = \overline A \cup \overline B$ |
| doppelte Komplementbildung | $\overline{\overline A} = A$                         |                                                      |

# Potenzmenge

Die Menge, die alle [Teilmengen](Mengen.md.md#teilmenge) einer Menge enthält
$$\begin{align*}
	M &= \{ 1,2,3 \}\\
	P(M) &= \{ \{ \}, \{1\}, \{2\}, \{3\}, \{ 1,2 \}, \{ 1,3 \}, \{ 2,3\}, \{ 1,2,3 \} \}\\
	|P(M)| &= 2^{|M|} = 2^{3} = 8
\end{align*}$$

Die Mächtigkeit einer Potenzmenge lässt sich mit $|P(M)= 2^{|M|} |$ berechnen

# Kartesisches Produkt

Die Menge aller geordneten Paare zweier Mengen A und B

Man benötigt 2 Mengen (es kann auch 2 mal die gleiche Menge sein)
Dann bildet an alle Paare so, dass die erste Komponente im Paar aus der ersten Menge und die zweite Komponente aus der zweiten Menge ist.
$$\begin{align*}
	A \times B = \{[a,b] : a \in A, b \in B \}
\end{align*}$$
