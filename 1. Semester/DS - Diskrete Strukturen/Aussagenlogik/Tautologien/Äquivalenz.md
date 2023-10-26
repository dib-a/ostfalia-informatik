---
tags:
  - 1-Semester
  - DS-Diskrete-Strukturen
  - Aussagenlogik
  - Tautologien
share: "true"
---
Äquivalenz ist eine [Bijunktion](../Logische%20Operatoren/Bijunktion.md#), die immer wahr ist ([Tautologien](./Tautologien.md#))

$A \Leftrightarrow B$ :
- A ist die notwendige und hinreichende Bedingung für B
- B ist die notwendige und hinreichende Bedingung für A

> [!Tip] hinreichende Bedingung
> Eine Bedingung ist hinreichend, wenn das Ereignis auftreten kann, wenn die Bedingung erfüllt ist, **aber auch sonst**

> [!Tip] notwendige Bedingung
> Eine Bedingung ist notwendig, wenn das Ereignis dann und nur dann auftreten kann, wenn die Bedingung erfüllt ist

Da gilt:
- $A \leftrightarrow B \Leftrightarrow (A \rightarrow B) \land (B \rightarrow A)$

folgt für jede [Tautologie](./Tautologien.md#) der Form
- $A \Leftrightarrow B = (A \Rightarrow B) \land (B \Rightarrow A)$

Bsp: "Eine Zahl ist dann und nur dann gerade, wenn sie durch 2 teilbar ist"
- die Teilbarkeit durch 2 ist eine notwendige und hinreichende Voraussetzung dafür, dass die Zahl gerade ist
	- eine Zahl kann dann und nur dann gerade sein, wenn sie durch 2 teilbar ist
- das die Zahl gerade ist, ist eine notwendige und hinreichende Bedingung dafür, dass eine Zahl durch 2 teilbar ist 
	- eine Zahl kann dann und nur dann durch 2 teilbar sein, wenn sie gerade ist

Da gilt:
- $A \rightarrow B \Leftrightarrow \lnot B \rightarrow \lnot A$

folgt für jede [Tautologie](./Tautologien.md#) der Form
- $A \Rightarrow B = \lnot B \Rightarrow \lnot A$

Bsp: aus der [Aussage](../Aussagen-und-Aussageformen.md#aussagen)
	- "Wenn eine Zahl durch 4 teilbar ist, dann ist sie auch durch 2 teilbar" wird
	- Wenn eine Zahl nicht durch 2 teilbar ist , dann ist sie auch nicht durch 4 teilbar

# Äquvalenzumformungen
Umformungen
- $\Leftrightarrow$ Beschreibt den Zusammenhang zwischen aufeinanderfolgenden bzw. umgeformten Gleichungen
- Wahrheitswert der Gleichung bleibt unverändert
- Bsp:

$$\begin{align}
	&& ax^4+bx&=-c \\ 
	\Leftrightarrow && ax^2+bx+c&= 0
\end{align}$$


> [!Warning] Häufiger Fehler
> - statt $\Leftrightarrow$ wird nur $\Rightarrow$ geschrieben
>	- ist falsch
>	- nur die halbe Wahrheit
