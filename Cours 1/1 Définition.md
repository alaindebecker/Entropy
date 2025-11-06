(1.1) Définition
================

On cherche à quantifier l'information apportée par l'observation d'une variable aléatoire. 

Or, il est naturel de penser que l'information apportée par l'observation conjointe de deux 
évenements indépendants $A$ et $B$ est la somme des informations apportées par chacun 
d'eux : $H(A \cap B) = H(A) + H(B)$. Et comme on a  $P(A \cap B) = P(A) P(B)$, car les évenements 
sont indépendants, il suffit d'en prendre les logarithmes pour avoir une information additive : 
$H(A \cap B) = \log(P(A \cap B)) = \log(P(A)) + \log(P(B)) = H(A)+H(B)$. 

L'information portée par la variable $X$ devant être quantifiée par un nombre unique qui dépend 
uniquement de sa distribution, et non des valeurs prises par $X$ en est ammené à définir l'entropie 
comme la moyenne des logarithme des probabilités élementaires $\log(P(X=a)) = \log(p_a)$. 

**Définition (Shannon, 1948):** *L'**entropie de Shannon** d'une variable aléatoire* $X$ *à valeur sur un ensemble* $A$*, 
est définie par*

$$\begin{aligned}
       H(X)   &= \sum_{x \in A} P(X=a) \log_2 \left( \frac{1}{P(X=a)} \right) \\
              &= \sum_{x \in A} p_a \log_2 \left( \frac{1}{p_a} \right) \\
              &= -\sum_{x \in A} p_a \log_2 {p_a}.
\end{aligned}$$

Les prochains chapitres sont consacrés à une redéfinition de l'entropie plus intuitive, basée sur 
ses propriétés élémentaire, et d'une discution sur le choix de la base du logarithme.

En attendant, citons immédiatement un lemme permettant de calculer l'entropie d'une distribution empirique.

**Lemme:** *Lorsque loi de la variable aléatoire* $X$ *est connue par un échantillon* $x_1, x_2, \cdots x_n$ 
*dans lequel la variable prend* $n_i$ *fois la valeur* $x_i$*, son entropie vaut*

$$H(x) = \log_2(n) - \frac 1 {n} \sum_i{n_i \log_2 n_i}, \quad \textit{dans laquelle} \quad n = \sum_i n_i.$$

La preuve consiste à réécrire la formule de Shannon avec $p_i=n_i/n$ :

$$ H(X) = \sum_i \frac{n_i}{n} \log \frac{n}{n_i} 
        = \frac{1}{n} \sum_i n_i ( \log n - \log n_i )
        = \frac{1}{n} \sum_i n_i \log n - \frac{1}{n} \sum_i n_i \log n_i
$$

Le lemme s'en déduit immédiatement en factorisant $\log n$ dans la première somme, 
puis en remarquant que $\sum n_i = n$.


Références:
-----------
- C. E. SHANNON, *A Mathematical Theory of Communication*, The Bell System Technical Journal, 
Vol. 27, pp. 379–423, 623–656, July, October, 1948.




