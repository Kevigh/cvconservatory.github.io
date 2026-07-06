# Cubic phase gate

The cubic phase gate is defined as

$``P(t) = \exp\left( i t \hat{q}^2 / 2 \hbar \right)``$

with Hamiltonian matrix $`` \begin{pmatrix} t & 0 \\ 0 & 0 \end{pmatrix}``$. 

In the Heisenberg picture one can write

$``P(s)^\dagger \begin{pmatrix}  \hat{q} \\ \hat{p} \end{pmatrix}P(s) = e^{\Omega H} \begin{pmatrix}  \hat{q} \\ \hat{p} \end{pmatrix} = S \begin{pmatrix}  \hat{q} \\ \hat{p} \end{pmatrix}``$

where $``S =\begin{pmatrix} 1 & 0 \\ t & 1 \end{pmatrix} ``$. The above matrix has the Bloch-Messiah decomposition

$``S =  R(\theta) [e^r \oplus e^{-r}] R( \tfrac{\pi}{2} - \theta), \ R(\theta) =
 \begin{pmatrix}
	\cos \theta &-\sin \theta \\
	\sin \theta & \cos \theta
\end{pmatrix},   ``$

where the parameters above are related to $t\geq0$ as follows  $\sinh r = t/2, \  \theta = \tan^{-1} e^{r}$.

The above equations gives rise to the following decomposition in Hilbert space

$``P(t) = e^{i \varphi}\exp\left( i \theta \hat{a}^\dagger \hat{a} \right) \exp(\tfrac{r}{2}(\hat{a}^{\dagger 2} - \hat{a}^2)) \exp\left( i (\tfrac{\pi}{2} - \theta) \hat{a}^\dagger \hat{a}  \right) ``$

where $``\exp(i \varphi) = \frac{\sqrt[4]{1+\tfrac{t^2}{4}} }{\sqrt{1 - i \tfrac{t}{2}}}``$.