---
tags:
  - 1-Semester
  - DS-Diskrete-Strukturen
  - Prädikatenlogik
share: "true"
---

Die Prädikatenlogik befasst sich inbesondere mit Wegen um aus Aussageformen Aussagen zu machen. Dies gelingt meist, indem man die Variablen mit Werten belegt.

# Quantifizierte Aussagen

- ist die [Aussageform](../Aussagenlogik/Aussagen-und-Aussageformen.md#aussageformen) für **alle** möglichen Variablenwerte wahr?
- ist die [Aussageform](../Aussagenlogik/Aussagen-und-Aussageformen.md#aussageformen) für **mindestens einen** möglichen Variablenwert wahr?

## All-Aussagen

$$\begin{align*}
	\forall (x \in M \mid P(x))
\end{align*}$$
Gesprochen: "Für alle x aus der Menge M gilt P(x)"

ist genau dann wahr, wenn für **alle** Belegungen von x aus der Menge M die Aussagen wahr sind.

$\forall$ : Allquantor

Synonyme: für alle, jede, immer
## Existenz-Aussagen

$$\begin{align*}
	\exists (x \in M \mid P(x))
\end{align*}$$
Gesprochen: "Es gibt ein x aus der Menge M, sodass P(x) gilt"

ist genau dann wahr, wenn für **mindestens eine** Belegungen von x aus der Menge M die Aussage wahr ist.

$\exists$ : Existenzquantor
Synonyme: gibt es eine

# Modellieren mit Quantoren

| Quantor | Variablen mit Mengenangabe | Prädikat |
| ------- | -------------------------- | -------- |
| $\forall\  / \ \exists$     | $x \in M$                    | $P(x)$     |

# Negation quantifizierter Aussagen

$$\begin{align*}
	&\not \forall & &=& \lnot \forall (x \in M \mid P(x)) & &\Leftrightarrow & & \exists(x \in M \mid \lnot P(x))\\
	&\not \exists & &=& \lnot \exists (x \in M \mid P(x)) & &\Leftrightarrow & &\forall(x \in M \mid \lnot P(x))
\end{align*}$$

**Schritt für Schritt**
1. Den Quantor umdrehen: aus $\forall$ wird $\exists$ und umgedreht
2. Das Prädikat negieren
3. Zur Überprüfung: Versprachlichen 

> [!NOTE] Beispiel 
>Aussage: Jeder versteht Logik: $\forall (m \in \text{Menschen} \mid m\  \text{versteht Logik})$ 
>Negation: Jemand versteht Logik nicht: $\exists (m \in \text{Menschen} \mid \lnot (m\  \text{versteht Logik}))$
>
>Es reicht zu zeigen, dass es einen Menschen gibt der die Logik nicht versteht, dann ist die Aussage bereits falsch

# Gebundene und freie Variablen

$$\exists (n \in \mathbb{N} \mid n^2 = n)$$
ist wahr, ohne das n mit einem Wert belegt wird.
Also ist dies eine [Aussage](../Aussagenlogik/Aussagen-und-Aussageformen.md#aussagen) und keine [Aussageform](../Aussagenlogik/Aussagen-und-Aussageformen.md#aussageformen).

- hier hat man nicht **die Freiheit** n mit einem Wert zu belegen das macht der Quantor für uns
	- es **muss** gelten n=1

$$\exists (n \in N \mid n < y)$$
- hier ist der Wahrheitswert nicht bekannt, da y variable **(frei)** ist

Variablen die innerhalb eines Ausdrucks an große Operatoren wie $\forall\ , \exists\ , \sum$ gebunden sind, nennt man gebunden

# Geschachtelte quantifizierte Aussagen

$$\begin{align*}
	\exists (k \in \mathbb{N} \mid \forall(n \in \mathbb{N} \mid k = n + 1))
\end{align*}$$

> [!Warning] Reihenfolge der Quantoren
> Die Reihenfolge der Quantoren ist wichtig
> $$\forall (x \in M \mid \exists (y \in N \mid P(x,y))) \nLeftrightarrow \exists ( y \in N \mid \forall (x \in M \mid P(x,y)))$$

==Diagram einfügen ACHTUNG open source???== --- fragen ob das aus dem Skript übernommen werden darf

## Vereinfachungen
Tritt derselbe Quantor mehrfach hintereinander auf, wir der nur einmal aufgeschrieben
$$\begin{align*}
	&\forall (x \in M, y \in N \mid P(x,y))\\ 
	\text{statt}\ &\forall ( x \in M \mid \forall (y \in N \mid P(x,y)))
\end{align*}$$
Sind die Mengen gleich, wird dies auch nur einmal aufgeschrieben
$$\begin{align*}
	&\forall (x, y \in M \mid P(x,y))\\ 
	\text{statt}\ &\forall ( x \in M, y \in M \mid P(x,y)))
\end{align*}$$
Wenn aus dem Kontext klar ist welche Menge gemeint ist, wird diese nicht mehr aufgeschrieben
$$\begin{align*}
	&\forall (x \mid P(x))\\ 
	\text{statt}\ &\forall (x \in M \mid P(x))
\end{align*}$$
# Quantoren als große Operatoren

Große Operatoren finden Verwendung beim mehrfachen Ausführen von [kommutativen](kommutativen.md#) und [assoziativen](assoziativen.md#) [binären Operatoren](bin%C3%A4ren%20Operatoren.md#)
#### Summenoperator
$$\begin{align*}
	\sum_{i=1}^{N}{a_i} = a_1 + a_2 + ... + a_{N-1} + a_N
\end{align*}$$
#### Produktoperator
$$\begin{align*}
	\prod_{i=1}^{N}{a_i} = a_1 \cdot a_2 \cdot ... \cdot a_{N-1} \cdot a_N
\end{align*}$$
#### Konjunktion
$$\begin{align*}
	\bigwedge_{i=1}^{N}{A_i} = A_1 \land A_2 \land ... \land A_{N-1} \land A_N
\end{align*}$$
Entspricht dem $\forall$
#### Disjunktion
$$\begin{align*}
	\bigvee_{i=1}^{N}{A_i} = A_1 \lor A_2 \lor ... \lor A_{N-1} \lor A_N
\end{align*}$$
Entspricht dem $\exists$

Indizes aus der Menge $\{ 1,...,N \}$
im Allgemeinen kann die Menge, aus der die Indizes gewählt werden, frei gewählt werden

Indexsymbol (hier i) ist eine gebundene Variable

##### Präzedenz

| Priorität |         1         |       2       |         3         |   4    |           5           |    6    |    7    |         8         |          9          |            10            | 11  | 12     | 13      | 14      |
|:---------:|:-----------------:|:-------------:|:-----------------:|:------:|:---------------------:|:-------:|:-------:|:-----------------:|:-------------------:|:------------------------:| --- | ------ | ------- | ------- |
|           | $\Leftrightarrow$ | $\rightarrow$ | $\leftrightarrow$ | $\lor$ | $\not\leftrightarrow$ | $\land$ | $\lnot$ | $\exists ,\bigvee$ | $\forall ,\bigwedge$ | $=, \not = , < ,> ,\leq, \geq$ | $+$ | $\sum$ | $\cdot$ | $\prod$ |

# [Tautologien](../Aussagenlogik/Tautologien/Tautologien.md#) und quantifizierte Aussagen

Definitionen und Theoreme lassen sich immer mit einem Allquantor beschreiben

#### Schlüsselwörter
- Jede
- ...ist genau dann..., wenn
## [Implikation](../Aussagenlogik/Tautologien/Implikation.md#)

$$\begin{align*}
	(A(x)\Rightarrow B(x)) &\Leftrightarrow (\forall (x \in U \mid A(x) \rightarrow B(x)) \Leftrightarrow \mathbb{1})\\
	\forall (x \in U \mid P(x)) &\Leftrightarrow \forall(x\in U \mid x\in U \rightarrow P(x))
\end{align*}$$

## [Äquivalenz](../Aussagenlogik/Tautologien/%C3%84quivalenz.md#)

$$\begin{align*}
	(A(x)\Leftrightarrow B(x)) &\Leftrightarrow (\forall (x \in U \mid A(x) \leftrightarrow B(x)) \Leftrightarrow \mathbb{1})\\
\end{align*}$$