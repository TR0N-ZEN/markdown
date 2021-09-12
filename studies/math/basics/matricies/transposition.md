**Transponierung**

Sei $A \in \mathbb{R}^{m \times n}$
$$
A =
	\left(\begin{matrix}
	a_{11} & \cdots & a_{1n} \\
	\vdots & \ddots & \vdots \\
	a_{m1} & \cdots & a_{mn}
	\end{matrix}\right)
$$
so ist die Transposition von $A$, also $A^T$ definiert als
$$
A^T =
	\left(\begin{matrix}
	a_{11} & \cdots & a_{m1} \\
	\vdots & \ddots & \vdots \\
	a_{1n} & \cdots & a_{mn}
	\end{matrix}\right)
$$
und $A^T \in R^{n \times m}$

Sei $A \in \mathbb{R}^{m \times n}$ und $B \in \mathbb{R}^{n \times s}$
$$
(AB)^T =
	\left(
		\left(\begin{matrix}
			a_{11} & \cdots & a_{1n} \\
			\vdots & \ddots & \vdots\\
			a_{m1} & \cdots & a_{mn}
		\end{matrix}\right)
		\left(\begin{matrix}
			b_{11} & \cdots & b_{1s} \\
			\vdots & \ddots & \vdots\\
			b_{n1} & \cdots & b_{ns}
		\end{matrix}\right)
	\right)^T
$$
$$
	=
	\left(
	\left(\begin{matrix}
		a_{11} b_{11} + \cdots + a_{1n} b_{n1} & \cdots & a_{11} b_{1s} + \cdots + a_{1n} b_{ns} \\
		\vdots & \ddots & \vdots \\
		a_{m1} b_{11} + \cdots + a_{mn} b_{n1} & \cdots & a_{m1} b_{1s} + \cdots + a_{mn} b_{ns}
	\end{matrix}\right)
	\right)^T
$$
$$
	=
	\left(\begin{matrix}
		a_{11} b_{11} + \cdots + a_{1n} b_{n1} & \cdots & a_{m1} b_{11} + \cdots + a_{mn} b_{n1}  \\
		\vdots & \ddots & \vdots \\
		a_{11} b_{1s} + \cdots + a_{1n} b_{ns} & \cdots & a_{m1} b_{1s} + \cdots + a_{mn} b_{ns}
	\end{matrix}\right)
$$
$$
	=
	\left(\begin{matrix}
		b_{11} a_{11} + \cdots + b_{n1} a_{1n} & \cdots & b_{11} a_{m1} + \cdots + b_{n1} a_{mn}  \\
		\vdots & \ddots & \vdots \\
		b_{1s} a_{11} + \cdots + b_{ns} a_{1n}  & \cdots & b_{1s} a_{m1} + \cdots + b_{ns} a_{mn} 
	\end{matrix}\right)
$$
$$
=
	\left(\begin{matrix}
		b_{11} & \cdots & b_{n1} \\
		\vdots & \ddots & \vdots\\
		b_{1s}& \cdots & b_{ns}
	\end{matrix}\right)
	\left(\begin{matrix}
		a_{11} & \cdots & a_{m1} \\
		\vdots & \ddots & \vdots\\
		a_{1n} & \cdots & a_{mn}
	\end{matrix}\right)
$$
$$
=B^TA^T
$$