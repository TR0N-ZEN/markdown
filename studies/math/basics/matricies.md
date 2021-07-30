Die allgemeine **m x n Matrix**
$$
A_{mn} = 
	\left(
	\begin{matrix}
	a_{11} & a_{12} & \cdots & a_{1n} \\
	a_{21} & a_{22} & \ddots & a_{2n} \\
	\vdots & \vdots & \ddots & \vdots\\
	a_{m1} & a_{m2} & \cdots & a_{mn}
	\end{matrix}
	\right)
	\tag{1}
$$
mit $\forall r,c \in \mathbb{N}: a_{rc} \in K$,

wobei wir nun schreiben $A_{mn} \in K^{m\times n}$

z.B. eine 3 x 3 Matrix
$$
A_{3,3} = 
	\left(
	\begin{matrix}
	a_{11} & a_{12} & a_{13} \\
	a_{21} & a_{22} & a_{23} \\
	a_{31} & a_{32} & a_{33}
	\end{matrix}
	\right)
	\tag{2}
$$
mit $\forall r,c \in \{1,2,3\}: a_{rc} \in \mathbb{R}$
,wobei wir nun schreiben $A \in \mathbb{R}^{3\times 3}$

,wobei eine konkrete Matrix $A_{k}$ so aussehen kann:
$$
A_{k} =
	\left(
	\begin{matrix}
	1 & 22 & 0 \\
	7 & 0 & 5 \\
	0 & 4 & 97
	\end{matrix}
	\right)
\tag{3}
$$

Matrizen der Form
$$
	v_{m} = 
	\left(
	\begin{matrix}
	a_{11} \\
	a_{12} \\
	\vdots \\
	a_{m1}
	\end{matrix}
	\right)
\tag{4}
$$
mit $\forall i \in \mathbb{N}: a_{i1} \in K$

werden **Vektoren** genannt
und wir schreiben nun $v_{m} \in K^m$.

Für Matrizen ist die **Matrizenaddition** wie folgt definiert:
$$
A_{mn} + B_{mn} = 
	\left(
	\begin{matrix}
	a_{11} & a_{12} & \cdots & a_{1n} \\
	a_{21} & a_{22} & \cdots & a_{2n} \\
	\vdots & \vdots & \ddots & \vdots\\
	a_{m1} & a_{m2} & \cdots & a_{mn}
	\end{matrix}
	\right)
	+
	\left(
	\begin{matrix}
	b_{11} & b_{12} & \cdots & b_{1n} \\
	b_{21} & b_{22} & \cdots & b_{2n} \\
	\vdots & \vdots & \ddots & \vdots\\
	b_{m1} & b_{m2} & \cdots & b_{mn}
	\end{matrix}
	\right)
	=
	\left(
	\begin{matrix}
	a_{11} + b_{11} & a_{12} + b_{12} & \cdots & a_{1n} + b_{1n} \\
	a_{21} + b_{21} & a_{22} + b_{22} & \cdots & a_{2n} + b_{2n} \\
	\vdots & \vdots & \ddots & \vdots\\
	a_{m1} + b_{m1} & a_{m2} + b_{m2} & \cdots & a_{mn} + b_{mn}
	\end{matrix}
	\right)
	\tag{5}
$$
mit $\forall r,c \in \mathbb{N}: a_{rc},b_{rc} \in K$.

Matrizen ist die Multiplikation mit einem Skalar, also die **Skalarmultiplikation** wie folgt definiert:
$$
sA_{mn} = s
	\left(
	\begin{matrix}
	a_{11} & a_{12} & \cdots & a_{1n} \\
	a_{21} & a_{22} & \cdots & a_{2n} \\
	\vdots & \vdots & \ddots & \vdots\\
	a_{m1} & a_{m2} & \cdots & a_{mn}
	\end{matrix}
	\right)
	=
	\left(
	\begin{matrix}
	sa_{11} & sa_{12} & \cdots & sa_{1n}\\
	sa_{21} & sa_{22} & \cdots & sa_{2n} \\
	\vdots & \vdots & \ddots & \vdots\\
	sa_{m1} & sa_{m2} & \cdots & sa_{mn}
	\end{matrix}
	\right)
	\tag{6}
$$
mit $\forall r,c \in \mathbb{N}: a_{rc},s \in K$.

Für Matrizen ist die **Matrizenmultiplikation** wie folgt definiert:
$$
A_{mn}  B_{ns} = 
	\left(
	\begin{matrix}
	a_{11} & \cdots & a_{1n} \\
	\vdots & \ddots & \vdots\\
	a_{m1} & \cdots & a_{mn}
	\end{matrix}
	\right)
	\left(
	\begin{matrix}
	b_{11} & \cdots & b_{1s} \\
	\vdots & \ddots & \vdots\\
	b_{n1} & \cdots & b_{ns}
	\end{matrix}
	\right)
$$
$$
	=
	\left(
	\begin{matrix}
	a_{11} b_{11} + a_{12} b_{21} + \cdots + a_{1n} + b_{n1} & \cdots & a_{11} b_{1s} + a_{12} b_{2s} + \cdots + a_{1n} + b_{ns} \\
	\vdots & \ddots & \vdots \\
	a_{m1} b_{11} + a_{m2} b_{21} + \cdots + a_{mn} + b_{n1} & \cdots & a_{m1} b_{1s} + a_{m2} b_{2s} + \cdots + a_{mn} + b_{ns}
	\end{matrix}
	\right)
	\tag{7}
$$
mit $\forall r,c \in \mathbb{N}: a_{rc},b_{rc} \in K$.
Eine andere Ideee der Vorstellungsentwicklung:
$$
A_{mn}  v_{n1} = 
	\left(
	\begin{matrix}
	a_{11} & \cdots & a_{1n} \\
	\vdots & \ddots & \vdots\\
	a_{m1} & \cdots & a_{mn}
	\end{matrix}
	\right)
	\left(
	\begin{matrix}
	b_{11} \\
	\vdots\\
	b_{n1}
	\end{matrix}
	\right)
$$
$$
	=
	\left(
	\begin{matrix}
	a_{11} b_{11} + a_{12} b_{21} + \cdots + a_{1n} + b_{n1}\\
	\vdots \\
	a_{m1} b_{11} + a_{m2} b_{21} + \cdots + a_{mn} + b_{n1}
	\end{matrix}
	\right)
	\tag{8}
$$

Sei
$$
A_{mn}  v_{ns} = 
	\left(
	\begin{matrix}
	a_{11} & \cdots & a_{1n} \\
	\vdots & \ddots & \vdots\\
	a_{m1} & \cdots & a_{mn}
	\end{matrix}
	\right)
	\left(
	\begin{matrix}
	b_{1s} \\
	\vdots\\
	b_{ns}
	\end{matrix}
	\right)
$$
$$
	=
	\left(
	\begin{matrix}
	a_{11} b_{11} + a_{12} b_{2s} + \cdots + a_{1n} + b_{ns}\\
	\vdots \\
	a_{m1} b_{1s} + a_{m2} b_{2s} + \cdots + a_{mn} + b_{ns}
	\end{matrix}
	\right)
	\tag{8}
$$
mit
$$
B_{ns} = \left(\begin{matrix}v_{n1} & \cdots & v_{ns}\end{matrix}\right)
$$
so ergibt sich $(7)$.