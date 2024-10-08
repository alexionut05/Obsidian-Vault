#### Exemplu
La inceputul unui joc de able, care este probabilitatea sa formam o 'poarta in casa'? Dar daca primul zar cade 6, se modifica probabilitatea?
$\Omega = \{1, 2, 3,...,6\} \times \{1, 2, 3,...,6\} = \{(i, j)|i, j = \overline{1,6}\}$

$\mathcal{F} = \mathcal{P}(\Omega), \mathbb{P}((i,j)) = \frac{1}{36}, \forall i, j = \overline{1,6}$

$A = \{"Poarta\ in\ casa"\}=\{(i, j)|i=\overline{1,6}\}\cup\{(i,j)|j=\overline{1,6}\}$

$B=\{(6,i)|i=\overline{1,6}\}$

$\mathbb{P}(A|B)=\frac{\mathbb{P}(A\cap B)}{\mathbb{P}(B)}=\frac{2}{6}=\frac{1}{3}$

#### Definitie (Probabilitati conditionate)
$\mathbb{P}(A|B)=\frac{\mathbb{P}(A\cap B)}{\mathbb{P}(B)}\Leftrightarrow\mathbb{P}(A\cap B)=\mathbb{P}(A|B)\cdot\mathbb{P}(B)=\mathbb{P}(B|A)\cdot\mathbb{P}(A)$

#### Definitie (Independenta)
Numim $A$ si $B$ independente daca $\mathbb{P}(A|B)=\mathbb{P}(A)\Leftrightarrow\mathbb{P}(A\cap B)=\mathbb{P}(A)\cdot\mathbb{P}(B)$.
Notatite $A\amalg B$

#### Exemple
i) Ce secvente de aruncari de monede este mai probabila?
	$CCCCCC$
	$CPPCPC$
	$PCPCPC$    
aceeasi probabilitate = $\frac{1}{2^6}$

ii) Aruncam 2 zaruri:
	$A="Primul\ \le2"$
	$B="Suma\ lor\ este\ 7"$
	$C="Al\ doilea\ este\ par"$
Care evenimente sunt independente?

$\Omega=\{1...6\}\times\{1...6\},\mathcal{F}=\mathcal{P}(\Omega)$
$A=\{(i,j)|i=\overline{1,2},j=\overline{1,6}\}$
$\mathbb{P}(A)=\frac{1}{3}$
$B=\{(i,j)|i,j=\overline{1,6},i+j=7\}$
$\mathbb{P}(B)=\frac{1}{6}$
$C=\{(i,j)|i=\overline{1,6},j\in\{2,4,6\}\}$
$\mathbb{P}(C)=\frac{1}{2}$

$\mathbb{P}(A\cap B)=\frac{1}{18}$
$A\amalg B, B\amalg C, A\amalg C$

#### Proprietati
Fie $(\Omega,\mathcal{F},\mathbb{P})$.
i) $A\amalg\emptyset$ si $A\amalg\Omega,\forall A\in\mathcal{F}$
ii) $A\amalg A\Leftrightarrow\mathbb{P}(A)\in\{0,1\}$
iii) Daca $A\amalg B$, $\mathbb{P}(A\cap B)=0\Leftrightarrow\mathbb{P}(A)=0$ sau $\mathbb{P}(B)=0$

#### Demonstratie
i) $\mathbb{P}(A\cap\emptyset)=\mathbb{P}(\emptyset)=0$
$\mathbb{P}(A)\cdot\mathbb{P}(\emptyset)=0\Rightarrow A\amalg\emptyset$
SAU
$\mathbb{P}(\emptyset|A)=\frac{\mathbb{P}(\emptyset|A)}{\mathbb{P}(A)}=0$

ii) $\mathbb{P}(A\cap A)=\mathbb{P}(A)\cdot\mathbb{P}(A)\Leftrightarrow\mathbb{P}(A)\in\{0,1\}$

iii) $\mathbb{P}(A\cap B)=\mathbb{P}(A)\cdot\mathbb{P}(B)$ (disjunctia e o relatie de dependenta)

#### Exemplu
La examen, Andrei invata un singur capitol din 14. Examen: alege la intamplare un capitol din 14 si concepe cu o intrebare grila cu 5 variante, raspuns unic.
a) Andrei se intreaba care este probabilitatea sa raspunda corect, alegand la intamplare o varianta daca nu stie?
Solutie:
$S = "Andrei\ stie\ sa\ raspunda", \mathbb{P}(S)=\frac{1}{14}$
$C="Andrei\ raspunde\ corect", \mathbb{P}(C)=?,\mathbb{P}(C|S^C)=\frac{1}{5}$
$\mathbb{P}(C|S)=1$
$\mathbb{P}(C)=\mathbb{P}((C\cap S)\cup(C\cap S^C))=\mathbb{P}(C\cap S)+\mathbb{P}(C\cap S^C)=\frac{1}{14}+\mathbb{P}(C|S^C)\cdot\mathbb{P}(S^C)=\frac{1}{14}+\frac{1}{5}\cdot\frac{13}{14}=\frac{9}{35}$

b) Profesorul vede ca Andrei a bifat corect si se intreaba care era probabilitatea ca Andrei sa fi ghicit si sa fi fentat examenul
Solutie:
$\mathbb{P}(S^C|C)=\frac{\mathbb{P}(S^C\cap C)}{\mathbb{P}(C)}=\frac{\mathbb{P}(C|S^C)\cdot\mathbb{P}(S^C)}{\mathbb{P}(C)}=\frac{1}{14}+\mathbb{P}(C|S^C)\cdot\mathbb{P}(S^C)=\frac{13}{18}$


