(1.1) Définition
================

On cherche à quantifier l'information apportée par l'observation d'une  variable aléatoire. 

Or, il est naturel de penser que l'information apportée par l'observation conjointe de deux 
évenements indépendants $A$ et $B$ est la somme des informations apportées par chacun 
d'eux : $H(A \cap B) = H(A) + H(B)$. Et comme on a  $P(A \cap B) = P(A) P(B)$, car les évenements 
sont indépendants, il suffit d'en prendre les logarithmes pour avoir une information additive : 
$H(A \cap B) = \log(P(A \cap B)) = \log(P(A)) + \log(P(B)) = H(A)+H(B)$. 

C<eci ammène à définir l'entropie d'une variable aléatoire quelconque comme étant la moyenne du 
logarithme des probabilités élementaires $\log(P(X=a)) = \log(p_a)$. 

**Définition:** *L'entropie de Shannon d'une variable aléatoire* $X$ *à valeur sur un ensemble* $A$*, 
est définie par*

$$\begin{aligned}
       H(X)   &= \sum_{x \in A} P(X=a) \log_2 \left( \frac{1}{P(X=a)} \right) \\
              &= \sum_{x \in A} p_a \log_2 \left( \frac{1}{p_a} \right) \\
              &= -\sum_{x \in A} p_a \log_2 {p_a}.
\end{aligned}$$

Les prochains chapitres sont consacrés à une vérification formelle de cette définition, ainsi que les 
raisons du choix du signe et de la base du logarithme.

En attendant, citons immédiatement un lemme pour calculer l'entropie 

**Lemme:** *Lorsque loi de la variable aléatoire* $X$ *est connue par un échantillon* $x_1, x_2, \cdots x_n$   

