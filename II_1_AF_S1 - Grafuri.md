---
tags:
  - graf
---
## Grafuri neorientate
- $G = (V, E)$
- $V =$ mulțimea nodurilor, finită și nevidă
- $E \subseteq V \times V$
- $E$ = mulțimea muchiilor (perechi neordonate -> $(x, y) = (y, x)$)
- Cardinalul maxim al lui $E = \frac{(|V| \cdot (|V| - 1))}{2}$
- $d(x)$ = gradul lui $x$ = numărul de muchiii incidente în $x$
- $\sum_{x\in V}^{} d(x) = 2 \cdot |E|$ => nr. par de muchii cu graf impar

## Grafuri parțiale
- $G = (V, E)$
- $G' = (V, E')$
- $E' \subseteq E$
- Câte grafuri parțiale are $G$? $2^{|E|}$

## Subgraf
- $G = (V, E)$
- $G'$ subgraf al lui $G$
- $G' = (V', E')$
- $V' \subseteq V$
- $E'$ mulțime din $E$ $eliminând muchiile cu extremități $V \backslash V'$
- Câte subgrafuri? $2^{|V|-1}$

## Lanț
- $(x_{1}, x_{2}, ..., x_{K})$
- $(x_{i}, x_{i+1}) \in E$
- Muchiile nu se repetă
- Lanț elementar = $\forall i, j; i \neq j \Rightarrow x_{i} \neq x_{j}$

## Ciclu
to be completed

## Matrice de adiacență
- $A[i][j]=1$, dacă $\exists$ muchia$(i, j)$
- Câte drumuri de lungime $k \ \exists$ între $(i, j)$?
- $A^k[i][j] =$ numărul de drumuri între $(i, j)$

## Listă de adiacență
to be completed

## Graf conex
- Cum verificăm dacă $G$ este graf conex? to be completed

## Probleme
1. Demonstrați că în $\forall$ graf $\exists x,y \in V$ astfel încât $d(x) = d(y)$.
Soluție: $(0, 1, 2, 3,... (n - 1))$, ultimul nod ar fi conectat la toate

2. Fie $G$ un graf neconex. Demonstrați că $\overline{G}$ este conex (complementul lui $G$)

x apartine R
$x \in \mathbb{R}$
