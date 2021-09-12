Die allgemeine **m x n Matrix**
$$
A_{mn} = 
	\left(	\begin{matrix}
		a_{11} & \cdots & a_{1n} \\
		\vdots & \ddots & \vdots\\
		a_{m1} & \cdots & a_{mn}
	\end{matrix}	\right)
\tag{1}
$$
mit $\forall r,c \in \mathbb{N}: a_{rc} \in K$ , wobei wir nun schreiben $A_{mn} \in K^{m \times n}$

>z.B. eine 3 x 3 Matrix
>$$
>A_{3,3} =
>	\left(	\begin{matrix}
>		a_{11} & a_{12} & a_{13} \\
>		a_{21} & a_{22} & a_{23} \\
>		a_{31} & a_{32} & a_{33}
>	\end{matrix}	\right)
>$$
>mit $\forall r,c \in \{1,2,3\}: a_{rc} \in \mathbb{R}$ , wobei wir nun schreiben $A \in \mathbb{R}^{3\times 3}$
>>,wobei eine konkrete Matrix $A_{k}$ so aussehen kann:
>>$$
>>A_{k} =
>>	\left(	\begin{matrix}
>>		1 & 22 & 0 \\
>>		7 & 0 & 5 \\
>>		0 & 4 & 97
>>	\end{matrix}	\right)
>>$$

Matrizen der Form
$$
	v_{m}
	=
	\left(	\begin{matrix}
		a_{11} \\
		a_{12} \\
		\vdots \\
		a_{m1}
	\end{matrix}	\right)
\tag{2}
$$

mit $\forall i \in \mathbb{N}: a_{i1} \in K$
werden **Vektoren** genannt und wir schreiben nun $v_{m} \in K^m$.

Für Matrizen ist die **Matrizenaddition** wie folgt definiert:
$$
A_{mn} + B_{mn} = 
		\left(	\begin{matrix}
		a_{11} & \cdots & a_{1n} \\
		\vdots & \ddots & \vdots\\
		a_{m1} & \cdots & a_{mn}
	\end{matrix}	\right)
	+
	\left(	\begin{matrix}
		b_{11} & \cdots & b_{1n} \\
		\vdots & \ddots & \vdots\\
		b_{m1} & \cdots & b_{mn}
	\end{matrix}	\right)
$$
$$
	=
	\left(	\begin{matrix}
		a_{11} + b_{11} & \cdots & a_{1n} + b_{1n} \\
		\vdots & \ddots & \vdots\\
		a_{m1} + b_{m1} & \cdots & a_{mn} + b_{mn}
	\end{matrix}	\right)
\tag{3}
$$
mit $ \forall r,c \in \mathbb{N}: a_{rc},b_{rc} \in K$ .

Matrizen ist die Multiplikation mit einem Skalar, also die **Skalarmultiplikation** wie folgt definiert:
$$
sA_{mn} = s
	\left(\begin{matrix}
	a_{11} & \cdots & a_{1n} \\
	\vdots & \ddots & \vdots\\
	a_{m1} & \cdots & a_{mn}
	\end{matrix}\right)
	=
		\left(\begin{matrix}
		sa_{11} & \cdots & sa_{1n}\\
		\vdots & \ddots & \vdots\\
		sa_{m1} & \cdots & sa_{mn}
	\end{matrix}\right)
\tag{4}
$$
mit $\forall r,c \in \mathbb{N}: a_{rc},s \in K$ .

Für Matrizen ist die **Matrizenmultiplikation** wie folgt definiert:
$$
A_{mn}  B_{ns}
$$
$$
=
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
$$
$$
	=
	\left(\begin{matrix}
		a_{11} b_{11} + \cdots + a_{1n} + b_{n1} & \cdots & a_{11} b_{1s} + \cdots + a_{1n} b_{ns} \\
		\vdots & \ddots & \vdots \\
		a_{m1} b_{11} + \cdots + a_{mn} b_{n1} & \cdots & a_{m1} b_{1s} + \cdots + a_{mn} b_{ns}
	\end{matrix}\right)
$$
mit $\forall r,c \in \mathbb{N}: a_{rc},b_{rc} \in K$ .

>Eine andere Idee der Vorstellungsentwicklung:
>$$
>	A_{mn}  v_{1} = 
>	\left(	\begin{matrix}
>		a_{11} & \cdots & a_{1n} \\
>		\vdots & \ddots & \vdots\\
>		a_{m1} & \cdots & a_{mn}
>	\end{matrix}	\right)
>	\left(	\begin{matrix}
>		b_{11} \\
>		\vdots\\
>		b_{n1}
>	\end{matrix}	\right)
>$$
>$$
>	=
>	\left(	\begin{matrix}
>		a_{11} b_{11} + \cdots + a_{1n} b_{n1}\\
>		\vdots \\
>		a_{m1} b_{11} + \cdots + a_{mn} b_{n1}
>	\end{matrix}	\right)
>$$
>
>Sei
>$$
>A_{mn}  v_{s} = 
>	\left(\begin{matrix}
>	a_{11} & \cdots & a_{1n} \\
>	\vdots & \ddots & \vdots \\
>	a_{m1} & \cdots & a_{mn}
>	\end{matrix}\right)
>	\left(\begin{matrix}
>	b_{1s} \\
>	\vdots\\
>	b_{ns}
>	\end{matrix}\right)
>$$
>$$
>	=
>	\left(\begin{matrix}
>	a_{11} b_{1s} + \cdots + a_{1n} b_{ns}\\
>	\vdots \\
>	a_{m1} b_{1s} + \cdots + a_{mn} b_{ns}
>	\end{matrix}\right)
>$$
wobei
$$
\forall v_{i} = 
	\left(\begin{matrix}
		b_{i1} \\ \vdots \\ w_{in}
	\end{matrix}\right):
	B_{ns} = \left(\begin{matrix}v_{1} & \cdots & v_{s}\end{matrix}\right)
$$
und
$$
\forall
w_{i} =
	\left(\begin{matrix}
		a_{i1} & \cdots & a_{in}
	\end{matrix}\right):
A_{mn} =
	\left(\begin{matrix}
		w_{1} \\ \vdots \\ w_{m}
	\end{matrix}\right)
$$
so ergibt sich $(5)$ wie folgt
$$
A_{mn} B_{ns} =
	\left(	\begin{matrix}
		w_{1}v_{1} & \cdots & w_{1}v_{s} \\
		\vdots & \ddots & \vdots \\
		w_{m}v_{1} & \cdots &  w_{1}v_{s}
	\end{matrix} \right)
$$
wobei $\forall i,j \in \mathbb{N}: w_{i}v_{j}$ das Skalarprodukt der Vektoren $w_{i}$ und $v_{j}$ ist.

---

**Eigenschaften der Matrizenmultiplikation**

**Assoziativität**
Für Matrizen ist die **Matrizenmultiplikation** wie folgt definiert:
$$
(A_{mn}  B_{ns}) C_{st}
$$
$$
=
	\left(
		\left(	\begin{matrix}
			a_{11} & \cdots & a_{1n} \\
			\vdots & \ddots & \vdots\\
			a_{m1} & \cdots & a_{mn}
		\end{matrix}	\right)
		\left(	\begin{matrix}
			b_{11} & \cdots & b_{1s} \\
			\vdots & \ddots & \vdots\\
			b_{n1} & \cdots & b_{ns}
		\end{matrix}	\right)
	\right)
	\left(	\begin{matrix}
		c_{11} & \cdots & c_{1t} \\
		\vdots & \ddots & \vdots\\
		c_{s1} & \cdots & c_{st}
	\end{matrix}	\right)
$$
$$
=
	\left(\begin{matrix}
		a_{11} b_{11} + \cdots + a_{1n} b_{n1} & \cdots & a_{11} b_{1s} + \cdots + a_{1n} b_{ns} \\
		\vdots & \ddots & \vdots \\
		a_{m1} b_{11} + \cdots + a_{mn} b_{n1} & \cdots & a_{m1} b_{1s} + \cdots + a_{mn} b_{ns}
	\end{matrix}\right)
	\left(
	\begin{matrix}
		c_{11} & \cdots & c_{1t} \\
		\vdots & \ddots & \vdots\\
		c_{s1} & \cdots & c_{st}
	\end{matrix}
	\right)
$$
