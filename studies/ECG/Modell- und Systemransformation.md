
Sei $v,x',y' \in \mathbb{R^2}$ und $a,b \in \mathbb{R}:$
$$
v = ax' + by' = 
	\left(\begin{matrix}
		x' & y'
	\end{matrix}\right)
	\left(\begin{matrix}
		a \\
		b
	\end{matrix}\right)
\tag{1}
$$
, wobei 
$v_{B} = \left(\begin{matrix}a \\ b\end{matrix}\right)$ **Koordinatenvektor** von v bezüglich der Basis B'
mit **Darstellungsmatrix** $D_{B'} = \left(\begin{matrix}x' & y'\end{matrix}\right)$ .

Also z.B.:
>Sei $v,x',y' \in \mathbb{R^2}$ und $a,b \in \mathbb{R}$ mit
>$$
>x'=
>	\left(\begin{matrix}
>	1 \\
>	0
>	\end{matrix}\right),
>	y'=
>	\left(\begin{matrix}
>	0 \\
>	1
>	\end{matrix}\right)
>$$
>$$
>v = a\left(\begin{matrix}1\\0\end{matrix}\right) + b\left(\begin{matrix}0\\1\end{matrix}\right)
>=
>	\left(\begin{matrix}
>		1 & 0 \\
>		0 & 1
>	\end{matrix}\right)
>	\left(\begin{matrix}
>		a \\
>		b
>	\end{matrix}\right)
>\tag{2}$$

oder

>Sei $v,x',y' \in \mathbb{R^2}$ und $ a,b \in \mathbb{R}$ mit
>$$
>x'=
>	\left(	\begin{matrix}
>		2 \\
>		1
>	\end{matrix}	\right),
>	y'=
>	\left(	\begin{matrix}
>		3 \\
>		1
>	\end{matrix}	\right)
>$$
>$$
>v = a\left(\begin{matrix}2\\1\end{matrix}\right) + b\left(\begin{matrix}3\\1\end{matrix}\right)
>=
>	\left(	\begin{matrix}
>		2 & 3 \\
>		1 & 1
>	\end{matrix}	\right)
>	\left(	\begin{matrix}
>		a \\
>		b
>	\end{matrix}	\right)
>\tag{3}
>$$

>Sei $v,x',y',x'',y'' \in \mathbb{R^2}$ und $ a,b,c,d \in \mathbb{R}$ mit
>$$
>x'=
>	\left(	\begin{matrix}
>		1 \\
>		0
>	\end{matrix}	\right),
>	y'=
>	\left(\begin{matrix}
>		0 \\
>		1
>	\end{matrix}	\right)
>$$
>$$
>x''=
>	\left(\begin{matrix}
>		2 \\
>		1
>	\end{matrix}\right),
>	y''=
>	\left(\begin{matrix}
>		3 \\
>		1
>	\end{matrix}\right)
>$$
>$$
>v=
>	\left(\begin{matrix}
>		1 & 0 \\
>		0 & 1
>	\end{matrix}\right)
>	\left(\begin{matrix}
>		a \\
>		b
>	\end{matrix}\right)
>	=
>	\left(\begin{matrix}
>		2 & 3 \\
>		1 & 1
>	\end{matrix}\right)
>	\left(\begin{matrix}
>		c \\
>		d
>	\end{matrix}\right)
>\tag{4}
>$$
>So ist $\left(\begin{matrix} a \\ b \end{matrix}\right)$ der Koordinatenvektor von v bezüglich $B'$
>mit $D_{B'} = \left(\begin{matrix} x' & y' \end{matrix}\right)$
>und $\left(\begin{matrix} c \\ d \end{matrix}\right)$ der Koordinatenvektor von v bezüglich $B''$
>mit $D_{B''} = \left(\begin{matrix} x'' & y'' \end{matrix}\right)$.
>Um $v_{B''}=\left(\begin{matrix} c \\ d \end{matrix}\right)$ unter Angabe von $v_{B'}=\left(\begin{matrix} a \\ b \end{matrix}\right)$, $D_{B'}$ und $D_{B''} zu berechnen nutze folgende Idee:
>$$
>	\left(\begin{matrix}
>		1 & 0 \\
>		0 & 1
>	\end{matrix}\right)
>	\left(\begin{matrix}
>		a \\
>		b
>	\end{matrix}\right)
>	=
>	\left(\begin{matrix}
>		2 & 3 \\
>		1 & 1
>	\end{matrix}\right)
>	\left(\begin{matrix}
>		c \\
>		d
>	\end{matrix}\right)
>\tag{5}
>$$
>$$
>	\left(\begin{matrix}
>		2 & 3 \\
>		1 & 1
>	\end{matrix}\right)^{-1}
>	\left(\begin{matrix}
>		1 & 0 \\
>		0 & 1
>	\end{matrix}\right)
>	\left(\begin{matrix}
>		a \\
>		b
>	\end{matrix}\right)
>	=
>	\left(\begin{matrix}
>		c \\
>		d
>	\end{matrix}\right)
>\tag{6}
>$$

Also allgemein:

$$
v =
	\left(	\begin{matrix}
		x' & y'
	\end{matrix}	\right)
	\left(	\begin{matrix}
		a \\
		b
	\end{matrix}	\right)
=
	\left(	\begin{matrix}
	x'' & y''
	\end{matrix}\right)
	\left(	\begin{matrix}
		c \\
		d
	\end{matrix}\right)
	\tag{7}
$$
$$
	\left(	\begin{matrix}
	c \\
	d
	\end{matrix}	\right)
	=
	\left(	\begin{matrix}
		x'' & y''
	\end{matrix}	\right)^{-1}
	\left(	\begin{matrix}
		x' & y'
	\end{matrix}	\right)
	\left(	\begin{matrix}
		a \\
		b
	\end{matrix}	\right)
\tag{8}
$$
Und um auch den Koordinatenvektor zu errechen, bei gegebener Basis $B'$
mit $D_{B'} = \left(\begin{matrix} x' & y' \end{matrix}\right)$
$$
 v_{B'} = 
	\left(	\begin{matrix}
		a \\
		b
	\end{matrix}	\right)
	=
	\left(	\begin{matrix}
		x' & y'
	\end{matrix}	\right)^{-1}
  v
\tag{9}
$$
lässt sich die invertierte Darstellungsmatrix nutzen.


---
Konkret zur Vorlesung Transformierung heißt das
wobei $M_{A}^B$ zwei Interpretationen hat...
* Systemtransformation von B nach A, also: $v_{A} = M_{A}^Bv_{B}$
* Modelltransformation im System A, mit Abbildung der Basis A auf B, also: $v_{A}' = M_{A}^Bv_{A}$

Wobei nach der Systemtransformation mit $(8)$ klar ist, dass $M_{A}^B = {(D_{A})}^{-1}D_{B}$, denn $v = D_{A}v_{A} = D_{B}v_{B}$

D.h. $M_{A}^B M_{B}^C = {(D_{A})}^{-1}D_{B} {(D_{B})}^{-1}D_{C} = {(D_{A})}^{-1}D_{C} = M_{A}^C$