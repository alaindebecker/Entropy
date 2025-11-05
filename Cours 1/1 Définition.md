(1.1) Définition
================

On cherche à quantifier l'information apportée par l'observation d'une  variable aléatoire. 

Or, il est naturel de penser que l'information apportée par l'observation conjointe de deux 
évenements indépendants $A$ et $B$ est la somme des informations apportées par chacun 
d'eux : $H(A \cap B) = H(A) + H(B)$. Et comme on a  $P(A \cap B) = P(A) P(B)$ pour les évenements 
indépendants, il suffit de prendre $H(A) = \log{P(A)}$ et $H(B) = \log{P(B})$ pour avoir
une information additive sur les évenements.

Maintenant, pour une 



**Définition** Si $X$ est une variable aléatoire sur un ensemble $A$, 
son *entropie de Shannon* est définie par

$$H(X) = \sum_{x \in A} P(X=a) \log_2 \left( \frac{1}{P(X=a)} \right).$$

On pose souvent $p_a = P(X=a)$, de sorte que cette formule se réécrit

$$H(X) = \sum_{x \in A} p_a \log_2 \left( \frac{1}{p_a} \right) 
       = - \sum_{x \in A} p_a \log_2 {p_a}. $$

Dans cette dernière expression, le signe $-$ vient du fait que $p_a\le1$
et donc que son logarithme est négatif.

Cette formule loin de tomber du ciel est la seule à vérifier un certain 
nombre de propriétés qui seront exposées un peu plus loin. L'idée de 
Shannon était de mesurer l'information apportée par le variable aléagtoire $X$.
