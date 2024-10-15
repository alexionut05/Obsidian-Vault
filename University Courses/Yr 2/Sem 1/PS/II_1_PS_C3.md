#### Observatii
1) Fie $A\subseteq\Omega$. $A$ si $A^C$ formeaza o partitie $\Omega$. Pentru $\forall B\in\mathcal{F}$, $B\cap A$ si $B \cap A^C$ formeaza o parititie $B:\mathbb{P}(B)=\mathbb{P}(B\cap A)+\mathbb{P}(B\cap A^C)=\mathbb{P}(B|A)\cdot\mathbb{P}(A)+\mathbb{P}(B|A^C)\cdot\mathbb{P}(A^C)$
2) Generalizare:  $\text{Fie }(A_{k})_{k=\overline{1,n}}\text{ partitie }\Omega\text{. }\mathbb{P}(B)=\mathbb{P}(B\cap A_{1})+...+\mathbb{P}(B\cap A_{n})=\sum_{k=1}^{n}\mathbb{P}(B|A_{k})\cdot\mathbb{P}(A_{k})\text{ (Probabilitatile totale)}$
3) Bajes: $\mathbb{P}(B|A)=\frac{\mathbb{P}(B\cap A)}{\mathbb{A}}=\frac{\mathbb{P}(A|B)\cdot\mathbb{P}(B)}{\mathbb{P}(A)}$

#### Exemplu
Iunie 2020: se estimeaza ca numarul real de bolnavi Covid era de 0.1% din populatia tarii.
1) Din 100 de bolnavi testati, 98 sunt depistati pozitiv (sensibilitatea testului).
2) Din 100 de sanatosi testati, 99 sunt depistati negativ (specificitatea testului).
Ma testez si ies pozitiv. Care este probabilitatea sa am Covid?
$\text{Fie }C=\text{"bolnav de Covid"},+=\text{"test pozitiv"},-=+^C,\mathbb{P}(C)=\frac{1}{1000}$
$\mathbb{P}(+|C)=0.98,\mathbb{P}(-|C^C)=0.99\Rightarrow\mathbb{P}(+|C^C)=0.01$
$\mathbb{P}(C|+)=\frac{\mathbb{P}(+|C)\cdot\mathbb{P}(C)}{\mathbb{P}(+)}=\frac{\mathbb{P}(+|C)\cdot\mathbb{P}(C)}{\mathbb{P}(+|C)\cdot\mathbb{P}(C)+\mathbb{P}(+|C^C)\cdot\mathbb{P}(C^C)}=\frac{\frac{98}{100}\cdot\frac{1}{1000}}{\frac{98}{100}\cdot\frac{1}{1000}+\frac{1}{100}\cdot\frac{999}{1000}}=\frac{98}{1097}=0.089$
Luam un esantion de 100000 oameni. (100 bolnavi, 999900 sanatosi)=>98 bolnavi depistati+, 999 sanatosi depistati+

$+_1=\text{"Testul 1 este pozitiv"},+_2=\text{"Testul 2 este pozitiv"}$
Avem $(+_1\indep +_2)|C$ dar nu $+_1\indep +_2$
$\mathbb{P}(C|+_1\cap +_2)=?$
$\mathbb{P}(C|+_1\cap +_2)=\frac{\mathbb{P}(+_1\cap +_2|C)\cdot\mathbb{P}(C)}{\mathbb{P}(+_1\cap +_2)}=\frac{\mathbb{P}(+_1|C)\cdot\mathbb{P}(+_2|C)\cdot\mathbb{P}(C)}{\mathbb{P}(+_1\cap +_2|C)\cdot\mathbb{P}(C)+\mathbb{P}(+_1\cap +_2|C^C)\cdot\mathbb{P}(C^C)}=...=0.9$
#### Definitie
$\newcommand{\indep}{\perp \!\!\! \perp}$**Independenta conditionata:** $A$ si $B$ sunt independente conditionat de $C$ daca $\mathbb{P}(A\cap B|C)=\mathbb{P}(A|C)\cdot\mathbb{P}(B|C)$. Notatie: $(A\indep B)|C$.

## Variabile aleatoare
Care este probabilitatea ca suma zarurilor sa fie 8 intr-un joc de Catan?
$\Omega=\{1...6\}^2,\mathcal{F}=\mathcal{P}(\Omega),$
$X:\Omega\rightarrow\{2,3,...,12\}$
$X((i,j)):=i+j,\forall i,j=\overline{1,6}$
Ne intereseaza:
$A=\{(i,j)\in\Omega|X((i,j))=8\}=X^{-1}(\{8\})=\{X=8\}$
$\mathbb{P}(A)=\mathbb{P}(X=8)=\frac{5}{36}$
$\mathbb{P}(X\in B)=?,B\subseteq S$
#### Definitie
Fie $(\Omega,\mathcal{F})$ si $(S,\mathcal{S})$ doua spatii masurabile.
Numim $X:\Omega\rightarrow\mathcal{S}$ variabila aleatoare daca $X^{-1}(B)=\{X\in B\}\in\mathcal{F},\forall B\in\mathcal{S}$
In plan: Daca $S$ este cel mult numarabil, $X$ discreta. Daca $S$ este infinit numarabila, $X$ continue

#### Definitie
Fie $X:\Omega\rightarrow S$ variabila aleatoare.
$\micro_x:\mathcal{S}\rightarrow[0,1]$ distributia lui x
$\micro_x(B):=\mathbb{P}(X\in B),\forall B\in\mathcal{S}$
#### Observatie
1) $\micro_x$ este o probabilitate pe $(S,\mathcal{S})$
	-> $\micro_x(S)=\mathbb{P}(x\in S)=\mathbb{P}(\Omega)=1$
	-> Fie $(B_n)_n$ disj. 2 cate 2. $\micro_x(\bigcup_{n}B_n)=\mathbb{P}(x\in\bigcup_{n}B_n)=\mathbb{P}(\bigcup_{n}\{x\in B_n\})=\sum_{n}\mathbb{P}(x\in B_n)$
2) $(\Omega,\mathcal(F),\mathbb{P})\xrightarrow{x}(S,\mathcal{S},\micro_x)$
3) Daca $S=\{x_1,x_2,...,x_n,...\}$ cel mult numarabila, $\mathcal{S}=\mathcal{P}(S)$
	$x:\Omega\rightarrow S$ v.a. discreta
	Fie $B\in\mathcal{S}=\mathcal{P}(S)\Rightarrow B=\bigcup_{x_n\in B}\{x_n\}$
	$\micro_n(B)=\mathbb{P}(x\in B)=\mathbb{P}(x\in\bigcup_{x_n\in B}\{x_n\})=\mathbb{P}\bigcup_{x_n\in B}=\sum_{x_n\in B}\mathbb{P}(x=x_n)=\sum_{x_n\in B}\micro_x(x_n)$
	$\micro_x$ este unic determinata de $(\micro_x(x_n))_{n\geq 1}$

#### Definitie
Fie $X:\Omega\rightarrow S=\{x_1,...,x_n,...\}$ v.a. discreta.
Numim $p:S\rightarrow[0,1]$ functia de masa
$p(x_n):=\micro_x(\{x_n\})=\mathbb{P}(X=x_n),\forall n\geq 1$ determina in mod unic distributia lui $X$
Notatie: $X~\begin{pmatrix}x_1&x_2&...&x_n&...\\p(x_1)&p(x_2)&...&p(x_n)&...\end{pmatrix}$
Catan: $X~\begin{pmatrix}2&3&4&5&6&7&8&9&10&11&12\\1/36&...\end{pmatrix}$

