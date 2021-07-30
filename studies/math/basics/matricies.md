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
	\tag{1}>$$
mit $\forall r,c \in \mathbb{N}: a_{rc} \in K$,

wobei wir nun schreiben $A_{mn} \in K^{m\times n}$

>z.B. eine 3 x 3 Matrix
>$$
A_{3,3} = 
	\left(
	\begin{matrix}
	a_{11} & a_{12} & a_{13} \\
	a_{21} & a_{22} & a_{23} \\
	a_{31} & a_{32} & a_{33}
	\end{matrix}
	\right)$$
>mit $\forall r,c \in \{1,2,3\}: a_{rc} \in \mathbb{R}$
>, wobei wir nun schreiben $A \in \mathbb{R}^{3\times 3}$
>>
>>,wobei eine konkrete Matrix $A_{k}$ so aussehen kann:
>>$$
A_{k} =
	\left(
	\begin{matrix}
	1 & 22 & 0 \\
	7 & 0 & 5 \\
	0 & 4 & 97
	\end{matrix}
	\right)$$

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
\tag{2}
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
	\tag{3}
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
	\tag{4}
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
	\tag{5}
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
	\tag{6}
$$

Sei
$$
A_{mn}  v_{ns} = 
	\left(\begin{matrix}
	a_{11} & \cdots & a_{1n} \\
	\vdots & \ddots & \vdots\\
	a_{m1} & \cdots & a_{mn}
	\end{matrix}\right)
	\left(\begin{matrix}
	b_{1s} \\
	\vdots\\
	b_{ns}
	\end{matrix}\right)
$$
$$
	=
	\left(\begin{matrix}
	a_{11} b_{11} + a_{12} b_{2s} + \cdots + a_{1n} + b_{ns}\\
	\vdots \\
	a_{m1} b_{1s} + a_{m2} b_{2s} + \cdots + a_{mn} + b_{ns}
	\end{matrix}\right)
	\tag{7}
$$
mit
$$
B_{ns} = \left(\begin{matrix}v_{n1} & \cdots & v_{ns}\end{matrix}\right)
$$
so ergibt sich $(5)$.

---

**Polynomfunktionen** lassen sich als ein Matrizenprodukt darstellen:

Sei $p(x)=a_{m}x^m+a_{m-1}x^{m-1}+\cdots+a_{1}x^1+a_{0}x^0$ bzw. $p(x)=a_{m}x^m+a_{m-1}x^{m-1}+\cdots+a_{1}x+a_{0}$ eine Polynomfunktion m-ten Grades mit $\forall i \in \mathbb{N},i<(m+1): a_{i} \in \mathbb{R}$, so stellt die folgende Matrix p(x) dar:
$$
	\left(\begin{matrix}
	a_{m}x^m + a_{m-1}x^{m-1} + \cdots + a_{1}x^1 +a_{0}x^0
	\end{matrix}\right)
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
	\tag{8}
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
	\tag{9}
$$
kurz:
$$Ax=b$$


Diese Schreibweise vereinfacht die Notation des Additionsverfahrens zum Lösen der Polynomfunktion.

Zur Überprüfung ihrer Bemühungen:
* Multipliziert man eine Zeile aus $A$ mit einem Skalar so muss in der gleichen Zeile in $b$ mit dem selben Skalar multipliziert werden
* Addiert man die i-te Zeile in $A$ auf die j-te Zeile in $A$, so muss die i-te Zeile in $b$ auf die j-te Zeile in $b$ addiert werden


>Die optimalste Form von a wäre eine Diagonalmatrix (alle Einträge außer auf der Hauptdiagonale sind 0):
>$$
D_{A} =
\left(\begin{matrix}
	r_{m} & 0 & \cdots & 0 & 0\\
	0 & r_{m-1}  & \cdots & 0 & 0\\
	\vdots & \vdots & \ddots & \vdots & \vdots\\
	0 & 0 & \cdots & r_{1} & 0 \\
	0 & 0 & \cdots & 0 & r_{0}
	\end{matrix}\right)
$$
