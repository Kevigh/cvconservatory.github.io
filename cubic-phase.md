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

We now compute the coherent-state matrix elements of $P(t)$

$\braket{\alpha^{*}|P(t)|\beta} = \braket{\alpha^{*}|e^{i \varphi}\exp\left( i \theta \hat{a}^\dagger \hat{a} \right) \exp(\tfrac{r}{2}(\hat{a}^{\dagger 2} - \hat{a}^2)) \exp\left( i (\tfrac{\pi}{2} - \theta) \hat{a}^\dagger \hat{a}  \right)|\beta},$

where we use the following identity to express the squeezing operator as 

$\exp{\left(\frac{r}{2}(a^{\dagger 2} - a^{2})\right)} = \exp{\left(\frac{\tanh{r}}{2}a^{\dagger 2}\right)}\exp{\left(-[a^{\dagger}a + 1/2]\ln{\cosh{r}}\right)}\exp{\left(-\frac{\tanh{r}}{2}a^{2}\right)},$

and a second identity to normal-order this expression

$\exp{(\theta a^{\dagger}a)} = :\exp{([\exp{(\theta)} - 1]a^{\dagger}a)}:,$

with $:(a^{\dagger}a)^{p}: = a^{\dagger p}a^{p}$.

Using these two identities, the decomposition of $P(t)$ takes the form

$P(t) = e^{i\varphi} \exp(i\theta a^{\dagger}a)\exp{\left(\frac{\tanh{r}}{2}a^{\dagger 2}\right)}\times:\frac{\exp{([1/\cosh{r}-1]a^{\dagger}a)}}{\sqrt{\cosh{r}}}:\times\exp{\left(-\frac{\tanh{r}}{2}a^{2}\right)}\exp{(i(\pi/2-\theta)a^{\dagger}a)}.$

Evaluating the matrix element $\braket{\alpha^{*}|\dots|\beta} = e^{i\varphi}\braket{\bar{\alpha}^{*}|\dots|\bar{\beta}}$ gives

$e^{i\varphi}\braket{\bar{\alpha}^{*}|\exp{\left(\frac{\tanh{r}}{2}a^{\dagger 2}\right)}\times:\frac{\exp{([1/\cosh{r}-1]a^{\dagger}a)}}{\sqrt{\cosh{r}}}:\times\exp{\left(-\frac{\tanh{r}}{2}a^{2}\right)}|{\beta}}$

where we have introduced the rotated labels $\bra{\bar{\alpha}^{*}} \equiv \bra{\alpha^{*}e^{-i\theta}} = \bra{\alpha^{*}}e^{i\theta a^{\dagger}a}$ and $\ket{\bar{\beta}} \equiv \ket{\beta e^{i(\pi/2 - \theta)}} = e^{i(\pi/2 - \theta) a^{\dagger}a}\ket{\beta}$ to simplify the expression. The resulting expression takes the form

$\sqrt{2}e^{i\varphi} \frac{\exp{[-\frac{1}{2}(\lvert \alpha \rvert^{2} + \lvert \beta \rvert^{2})]}}{\sqrt[4]{4+t^{2}}} \exp{\left(-\frac{1}{2} \begin{bmatrix} \alpha & \beta \end{bmatrix} \begin{bmatrix} f & g \\ g & f^{*} \end{bmatrix} \begin{bmatrix} \alpha \\ \beta \end{bmatrix} \right)}$

where we used the overlap of two coherent states $\braket{\bar{\alpha}^{*}|\bar{\beta}} = \exp{(-\frac{1}{2}(|\alpha|^{2} + |\beta|^{2} - 2\bar{\alpha}\bar{\beta}))}$, and the functions $f$ and $g$ are given by

$\begin{aligned} 
f &= -\tanh{r}e^{2i\theta}, \\
g &= -\frac{i}{\cosh{r}} ,
\end{aligned}$

or, in terms of the parameter $t$

$\begin{aligned} 
f &= \frac{t(t - 2i)}{4 + t^{2}}, \\
g &= - \frac{2i}{\sqrt{4 + t^{2}}}.
\end{aligned}$