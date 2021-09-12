
**Polynomfunktionen** lassen sich als ein Matrizenprodukt darstellen:

Sei $p(x)=a_{m}x^m+a_{m-1}x^{m-1}+\cdots+a_{1}x^1+a_{0}x^0$ bzw. $p(x)=a_{m}x^m+a_{m-1}x^{m-1}+\cdots+a_{1}x+a_{0}$ eine Polynomfunktion m-ten Grades mit $\forall i \in \mathbb{N},i<(m+1): a_{i} \in \mathbb{R}$, so stellt die folgende Matrix p(x) dar:
$$
	\left(\begin{matrix}
	a_{m}x^m + a_{m-1}x^{m-1} + \cdots + a_{1}x^1 +a_{0}x^0
	\end{matrix}\right)
$$
$$	
	=
	\left(\begin{matrix}
	a_{m} & a_{m-1} & \cdots & a_{1} & a_{0}
	\end{matrix}
	\right)
	\left(
	\begin{matrix}
	x^m \\
	x^{m-1}\\
	\vdots \\
	x^1 \\
	x^0
	\end{matrix}\right)
	\tag{7}
$$

Seien m verschiedene $p(x_{i})$ und $a_{i}$ gegeben so kann man als Matrixprodukt schreiben:
$$
	\left(\begin{matrix}
	a_{m} & a_{m-1} & \cdots & a_{1} & a_{0}\\
	\vdots & \vdots & \ddots & \vdots & \vdots\\
	a_{m} & a_{m-1} & \cdots & a_{1} & a_{0}
	\end{matrix}\right)
	\left(\begin{matrix}
	x^m \\
	x^{m-1}\\
	\vdots \\
	x^1 \\
	x^0
	\end{matrix}\right)
	=
	\left(\begin{matrix}
	p(x_{m}) \\
	p(x_{m-1})\\
	\vdots \\
	p(x_{1}) \\
	p(x_{0})
	\end{matrix}\right)
	\tag{8}
$$
kurz:
$$Ax=b$$


Diese Schreibweise vereinfacht die Notation des Additionsverfahrens zum Lösen der Polynomfunktion.

Zur Überprüfung ihrer Bemühungen:
* Multipliziert man eine Zeile aus $A$ mit einem Skalar so muss in der gleichen Zeile in $b$ mit dem selben Skalar multipliziert werden
* Addiert man die i-te Zeile in $A$ auf die j-te Zeile in $A$, so muss die i-te Zeile in $b$ auf die j-te Zeile in $b$ addiert werden


>Die optimalste Form von a wäre eine Diagonalmatrix (alle Einträge außer auf der Hauptdiagonale sind 0):
>$$
>D_{A} =
>\left(\begin{matrix}
>	r_{m} & 0 & \cdots & 0 & 0\\
>	0 & r_{m-1}  & \cdots & 0 & 0\\
>	\vdots & \vdots & \ddots & \vdots & \vdots\\
>	0 & 0 & \cdots & r_{1} & 0 \\
>	0 & 0 & \cdots & 0 & r_{0}
>	\end{matrix}\right)
>$$