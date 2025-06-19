> Содержание:
	Гл.1 Введение — стр. 1-64
    Гл.2 — стр. 64-106
	Гл.3 Эллиптические уравнения -- стр. 107-148
	Гл.4 Гиперболические и параболические уравнения — стр. 148-180

## Определения
 $$
(1) \sum_{i,j=1}^n a_{ij}(x) \frac{\partial^2 u}{\partial x_i \partial x_j}
+ \sum_{i=1}^n a_i(x) \frac{\partial u}{\partial x_i}
+ a_0(x) u = f(x), \quad x \in G \subseteq \mathbb{R}^n
$$
-  Уравнение (1) называется **гиперболическим** в точке $x^0 \in G$, если оно имеет 1 положительное (> 0) собственное значение  матрицы А и все остальные отрицательные или наоборот
-  Уравнение (1) называется **гиперболическим** в области G, если оно гиперболическое $\forall x^0 \in G$
-  Уравнение (1) называется **параболическим** в точке $x^0 \in G$, если количество нулевых собственных значений матрицы А больше 0.
-  **Параболичность** в области определяется аналогично гиперболичности.
-  Уравнение (1) называется **эллиптическим** в точке $x^0 \in G$, если все собственные значения в матрице А одного знака.
-  **Эллиптичность** в области определяется аналогично гиперболичности.
-   $$(4) \sum_{k=1}^{n^+(x^0)} \frac{\partial^2 \tilde{u}}{\partial y_k^2}
- \sum_{k=n^+(x^0)+1}^{n^+(x^0)+n^-(x^0)} \frac{\partial^2 \tilde{u}}{\partial y_k^2}
	+ Φ(y,\tilde{u},∇\tilde{u}) = 0 \text{ - канонический вид уравнений (1)}$$
- $$(1) \sum_{|\alpha \le m|} a_{\alpha} D^{\alpha}_x u = f(x), x \in G \subseteq R^n$$
 - $$\quad \left. \frac{\partial^k u}{\partial \nu^k} \right|_{S} := \sum_{|\beta| = k} \frac{k!}{\beta!} \, \nu^\beta D^\beta_x u \bigg|_{S} \text{ - производная по вектору нормали}$$
 -  $$D_{x_j} \rightarrow \xi_i : L_m(x, \xi) = \sum_{|\alpha| \le m}a_{\alpha}(x)\xi^{\alpha} \text{ - называется характеристическая форма оператора}$$
 - (стр. 13) Задачей Коши называется нахождения решения уравнения, удовлетворяющего начальным условиям}  ![[Pasted image 20250614220844.png]]
- (17) **Характеристическая поверхность** для оператора $L_m(x, D_x)$ (уравнения $L_m(x, D_x)u = f(x)$)![[Pasted image 20250615180504.png]]
- Вектор $\xi \in R^n$ **имеет характеристическое направление** для оператора $L_m(x, D_x)$ ($L_m(x, D_x)u = f(x)$) в точке $x^0$, если $L_m^0(x^0, \xi) = 0$ 
- Поверхность  S $-$ **характеристическая поверхность** для оператора $L_m$, если вектор нормали $\nu_kS$ в $\forall x \in S$ имеет характеристическое направление для $L_m(x, D_x)$
- (22) **Функция** V(y) называется **аналитической** в окрестности $y^0$, если ![[Pasted image 20250615183516.png]]
- Оператор $L_m(D_t. D_x)$ удовлетворяет **условию Адамара**, если ![[Pasted image 20250615183743.png]]
- (42) Оператор $L^*_2(x,y,D_x,D_y) = D^2_{xy}-aD_x-bD_y+[c-a_x-b_y]I$ называется **сопряженным** к оператору $L_2(x,y,D_x,D_y)$ 
- Функция Ришона и область зависимости решения![[Pasted image 20250615192713.png]]
- Задача Гурса - задача (17), сопряженная к задаче Коши (4), где u - решение задачи Коши, v - решение задачи Гурса![[Pasted image 20250615204115.png]]
- (44) **Краевая задача** для уравнения частных производных - задача на отыскание решения уравнения вида![[Pasted image 20250615204326.png]]
- Краевая задача (1), (2) называется корректной, когда:
	1. $\exists$ решение из класса V (где мы ищем решение, например в $W^1_2(G)$) для $\forall f, \psi, \dots,\psi_{\mu}$ из класса F (правые части)
	2. решение единственное в классе V
	3. решение непрерывно зависит от $f, \psi, \dots, \psi_{\mu}$ из класса  F
- (65) $\text{supp u} = \{x \in G : u(x)\ne 0\}$ - носитель u
- u называется финитной, если:
	1. supp u $\subset$ G
	2. supp u - ограниченное множество
- (67) Будем говорить, что u $\in L_{loc}(G)$ является **локально суммируемой** функцией, если $\forall$ ограниченной области $G'$ : $\overline{G'} \subset G$ u(x) $\in L_1(G')$ 
- Последовательность $\{u_n(x)\}$, $u_n(x) \in L_{loc}(G)$, $u \in L_{loc}(G)$. Будем говорить, что **$u_n(x)$ стремится к функции u(x) в $L_{loc}(G)$**, если $\forall$ ограниченной $G'$ : $\overline{G'} \subset G$ $||u_n - u, L_1(G)|| \xrightarrow[n \rightarrow \infty]{}0$ и пишем $u_n \xrightarrow[n \rightarrow \infty]{}u \text{ в } L_{loc}(G)$ 
- $\omega(t) \in C^{\infty}(R)$, $\omega(t)$ - четная. $\omega(t) \ge 0$, более того $\omega(t) = \begin{cases} > 0, |t| < 1 \\ = 0, |t| \ge 1 \end{cases}$ 
- Функция $\omega_h(x) = ch^{-n}\omega(\frac{|x|^2}{h^2})$  называется **усредняющим ядром**, если $\int_{R^n}\omega_h(x)dx = 1$ где  $h > 0$ - параметр усреднения, $x \in R^n$, $c = const$ 
- (69) Функция $u_h(x)$,  $x \in R^n$, $u_h(x) = \int_{R^n}\omega_h(x-y)\overline{u}(y)dy$ называется **средней функцией для u(x)** $\in L_p(G)$, где $\omega_h(x)$ - усредняющее ядро, h > 0 - параметр усреднения, $\overline{u}(x)=\begin{cases} u(x), x \in G \\ 0, x \in R^n\backslash G\end{cases}$ 
- Оператор, сопоставляющий функции u(x) ее среднюю $u_h(x)$ называется **оператором усреднения** (усредняющим оператором)
### Преобразование Фурье
- (72) Множество $S(R^n)$ - **множество быстроубывающих функций**, стремящихся к нулю вместе со своими производными быстрее любой степени $|x^{-k}|$ на бесконечности. То есть $\forall \alpha,\beta$ - мультииндексов $x^{\alpha}D_x^{\beta}\phi(x) \xrightarrow[|x|\rightarrow+\infty]{}0$ $(\phi(x) \in S(R^n))$ 
- **Сходимость в S:** $\phi^n \in S$ сходится к $\phi$ из S в S, если $\forall \alpha,\beta$ $x^{\alpha}D_x^{\beta}\phi^n(x) \underset{n \rightarrow \infty}{\Rightarrow} x^{\alpha}D_x^{\beta}\phi(x)$   равномерно по x. $C^{\infty} \subset S(R^n)$ - быстроубывающие функции. Например, $e^{-\frac{|x|^2}{2}} \in S(R^n)$, но $\notin C^{\infty}$ 
- Функция $\hat{u}(\xi) = \frac{1}{(\sqrt{2\pi})^n}\int_{R^n}e^{-ix\xi}u(x)dx$, $\xi \in R^n$ называется **преобразованием Фурье функции** $u(x) \in S(R^n)$
- Оператор, сопоставляющий функции её преобразование Фурье $\hat{u}$, называется **оператором Фурье** 
$$
\hat{u}(\xi) = F[u](\xi)
$$
- (74) $\check{\nu}(x) = (\sqrt{2\pi})^{-n}\int_{R^n}e^{ix\xi}\nu(\xi)d\xi$ называется обратным преобразованием Фурье функции $\nu(\xi) \in S(R^n)$
- Обратный оператор Фурье, сопоставляющий функции $\nu(\xi) \rightarrow \check{\nu}(x)$ определяется аналогично оператору Фурье
$$
\check{\nu}(x) = \underset{\xi \rightarrow x}{F^{-1}}[\nu](x)
$$
- Иное определение преобразования Фурье через сходимость ![[Pasted image 20250616022333.png]]
- (81) $\alpha = (\alpha_1, \dots, \alpha_n)$ - зафиксированный мультииндекс, $u(x) \in L_{loc}(G)$, $\nu(x) \in L_{loc}(G)$ и для $\forall \phi \in C^{\infty}_0(G)$ выполняется $\int_G u(x)D_x^{\alpha}\phi(x)dx = (-1)^{\alpha}\int_G \nu(x)\phi(x)dx$. Тогда функция $\nu(x)$ называется **обобщенной производной** функции $u(x)$ в области G  и обозначается $\nu(x)=D_x^{\alpha}u(x)$
- (89) $1 \le p < \infty$, $G \subseteq R^n$, $l \in N$, $u(x) \in L_p(G)$: $\exists \text{обобщенная производная} \underset{|\alpha| \le l}{D_x^{\alpha}u}$ в G, $D_u^{\alpha}u \in L_p(G)$. Линейное множество $\sum_{|\alpha| \le l}||D_x^{\alpha}u, L_p(G)||$  - линейное нормированное пространство $W^l_p(G)$ - **Соболевское пространство**. Метрики:
$$
\begin{align*}
||u, W^l_p(G)|| = \sum_{|\alpha| \le l}||D_x^{\alpha}u, L_p(G)||  \\
||u, W^l_p(G)|| = (\sum_{|\alpha| \le l}||D_x^{\alpha}u, L_p(G)||^p)^{\frac{1}{p}}
\end{align*}
$$

- (91) Рассматриваем множество функций из $C_0^{\infty}(G)$ $\sum_{|\alpha| \le l}||D_x^{\alpha}u, L_p(G)||$. $\overset{\circ}{W^l_p}(G)$ - пополнение $C_0^{\infty}(G)$ по норме Соболевского пространства
$$
||u, \overset{\circ}{W^l_p}(G)|| = ||u, W^l_p(G)|| = \sum_{|\alpha| \le l}||D_x^{\alpha}u, L_p(G)||  \\
$$
-  TODO: след функции 
### Теоремы вложения
- (99) Будем говорить, что линейное нормированное **пространство $B_1$ вложено в линейное нормированное пространство $B_2$**, $B_1 \hookrightarrow B_2$, если 
	1. $B_1 \subset B_2$
	2. $||u, B_2|| \le C||u, B_1||$
	Пример:
	![[Pasted image 20250616153702.png]]
### Эллиптические уравнения
![[Pasted image 20250616154651.png]]
- (107) Задача Дирихле (2) для эллиптического уравнения, 1-я краевая задача для уравнения (1)
$$
\begin{cases}
div(k(x)\nabla{u}) - a(x)u = f(x) \\ 
\left. u\right|_{\partial G} = \phi(x'), \quad x \in \partial G
\end{cases}
$$
- Задача Неймана (3) для эллиптического уравнения, 2-я краевая задача для уравнения (1) 
$$
\begin{cases}
div(k(x)\nabla{u}) - a(x)u = f(x) \\ 
\left. \frac{\partial u}{\partial \nu}\right|_{\partial G} = \psi(x'), x \in \partial G
\end{cases}
$$
- Функция $u(x) \in W^1_2(G)$ называется обобщенным решением задачи Дирихле (2) при $f \in L_2(G), \quad \phi \in L_2(\partial G)$, если $\forall v \in \overset{\circ}{W^1_2}(G)$ выполняется равенство 
$$
(4) \int_G\left[ k(x)\nabla u\nabla v + a(x)uv \right]dx = -\int_G fvdx
$$, где $\left. u \right|_{\partial G} = \phi(x'), \quad x' \in \partial G$ 
- Если $\phi \equiv 0$, тогда $u \in \overset{\circ}{W^1_2}(G)$ - обобщенное решение задачи Дирихле (2) при выполнении интегрального равенства (4)
- Функция $u(x) \in W^1_2(G)$ называется обобщенным решением Задачи Неймана (3) при $f \in L_2(G)$, $\psi \in L_2(\partial G)$, если
$$
\int_G \left[k(x)\nabla u \nabla v + a(x)uv \right]dx - \int_G k(x)\psi(x)u(x)dx = -\int_G fvdx
$$
- Пусть $\psi \equiv 0$. Функция $u(x) \in W^1_2(G)$ называется обобщенным решением Задачи Неймана при $f \in L_2(G)$, если $\forall v \in W^1_2(G)$ выполняется равенство (4)
### Уравнения Лапласа (118)
- Функция 
$$
\epsilon_n(x) = 
\begin{cases}
	\frac{1}{2\pi}ln|x|, \quad n = 2 \\
	- \frac{1}{\delta-n(1)(n-2)|x|^{n-2}}, \quad n \ge 3
\end{cases}
$$
	называется **фундаментальным решением уравнения Лапласа**, где $\delta_n(1)$ - площадь поверхности единичной сферы $S_n = \int_{|x|=n}1dS_n$ 
- (122) Вещественно значащая функция $u(x)$ называется гармонической в области G, если $u(x) \in C^2(G)$ и удовлетворяет уравнению Лапласа в каждой точке $x \in G$ (является решением уравнения Лапласа в области G)
#### Классическое решение задачи Дирихле для уравнения Пуассона и Лапласа
- (126) Функцией Грина краевой задачи Дирихле 
$$
\begin{cases}
	\Delta u = f(x), \quad x \in G, \quad G - \text{ограниченная область} \\
	\left. u \right|_{\partial G} = \phi(x'), \quad x' \in \partial G
\end{cases}
$$
	называется $g(y,x) = \tilde{g}(y, x) - \epsilon_n(x-y)$ , $\epsilon_n$ - фундаментальное решение уравнения Пуассона, $y \in \overline{G}$, $x \in G$, удовлетворяющее следующим условиям:
	1. $\Delta \tilde{g}$ = 0, $\forall x \in G$ 
		$\tilde{g} \in C^2(\underset{\text{см. G по y}}{G_y})\cap C(G)$  
	2. $\begin{cases}\left. g \right|_{y \in \partial G} = 0 \\ \left. \tilde{g} \right|_{y \in \partial G} = \left. \epsilon_n(x - y) \right|_{y \in \partial G} \end{cases}$  
- Функцией Грина внешней краевой Задачи Дирихле для шара называется $g(y,x) = \tilde{g}(y,x) - \epsilon_n(x - y)$, где
$$
\tilde{g}(y,x):
\begin{cases}
	\Delta_y \tilde{g} = 0, \quad |y| > r \\
	\left. \tilde{g} \right|_{|y|=r} = \left. \epsilon_n(x-y) \right|_{|y|=r}
\end{cases}
$$
- (132) Неравенство Гарнака![[Pasted image 20250617143009.png]]
#### Метод потенциалов
- (134) Внутренняя задача Дирихле
$$
(D^+)
\begin{cases}
	\Delta u = 0, \quad u \in G, \quad G - \text{ограниченная область} \subset R^n \\
	\left. y \right|_{\partial G} = \phi(x')
\end{cases}
$$
	нас будут интересовать такие классические решения: $u(x) \in C^2(G)\cap C(\overline{G})$
- Внешняя задача Дирихле
$$
(D^-)
\begin{cases}
	\Delta u = 0, \quad  x \in \overset{G_1}{\overbrace{R^n \backslash \overline{G}}}, \quad G - \text{ограниченная} \\ 
	\left. u \right|_{\partial G} = \phi(x') \\
	\underset{\overline{\text{Это дает ед-ть решения}}}{u \xrightarrow[|x| \rightarrow \infty]{}0} \quad (n \ge 3) \\
	u \le c, \quad n = 2
\end{cases}
$$
	$u(x) \in C^2(G_1)\cap C(\overline{G}_1)$ 
- (138) $u(x) \in C^1(G)$, граничная область класса $C^1$. Будем говорить, что $\exists$ правильная нормированная прямая на $\partial G$, если $\forall x^0 \in \partial G$![[Pasted image 20250617163823.png]]
- Внутренняя задача Неймана
$$
(N^+)
\begin{cases}
	\Delta u = 0, \quad x \in G, \quad G - \text{ограниченная гладкая  с границей } C^2 \\
	\left. \frac{\partial u}{\partial \nu}\right|_{\partial G} = \phi(x')
\end{cases}
$$
	$u \in C^2(G)\cap C(\overline{G})$ и $\exists$ правильная нормированная прямая на $\partial G$ 
- Внешняя задача Неймана
$$
(N^-)
\begin{cases}
	\Delta u = 0, \quad x \in G_1 = R^n \backslash G, \quad G - \text{ограниченная} \\
	\left. \frac{\partial u}{\partial \nu} \right|_{\partial G} = \phi(x') \\
	u \xrightarrow[|x| \rightarrow \infty]{}0, \quad n \ge 3 \\
	|u| \le c, \quad n = 2
\end{cases}
$$
	$u(x) \in C^2(G_1)\cap C(\overline{G}_1)$ и $\exists$ правильная нормированная прямая на $\partial G$
- **Потенциал простого слоя**
$$
P_1(x) = \frac{1}{4\pi}\int_{\partial G}\frac{\alpha(y)}{|x-y|}dS_y, \quad \alpha(y) \in C(\partial G) 
$$
- **Потенциал двойного слоя**
$$
P_2(x) = \frac{1}{4\pi}\int_{\partial G}\beta(y)\frac{\partial}{\partial \nu_y}\left( \frac{1}{|x-y|} \right)dS_y, \quad \beta(y) \in C(\partial G)
$$
- (145) **Фредгольмова пара**![[Pasted image 20250617174006.png]]
## Параболические уравнения. Уравнения теплопроводности. Принцип максимума (минимума)
- Классическим решением задачи
$$
\begin{cases}
	u_t - \Delta u = 0, \quad Ц_T = \left\{(t,x), \quad 0 < t \le T, \quad x \in \underset{\text{огр. обл.}}{G} \subset R^n \right\} \\
	\left. u \right|_{t = 0} = \phi(x) \\
	\left. u \right|_{S_{бок.}} = \chi(t,x), \quad (t,x) \in S_{б.} = \left\{ x \in \partial G, \quad 0 < t \le T\right\}
\end{cases}
$$
	называется функция u(t, x):
	1. $u \in C(Ц_T)$
	2. $\exists u_t, u_{x_j}, u_{x_i x_j} \in C(Ц_T)$ 
	3. При подстановке в задачу выше верно равенство
## Первая краевая задача в цилиндрической области для волнового уравнения. Метод Галеркина
- Функция $u \in W^1_2(Ц_T)$ - обобщенное решение краевой задачи![[Pasted image 20250617184055.png]]
	если![[Pasted image 20250617184129.png]]
- Функция $u \in W^1_2(Ц_T)$ - обобщенное решение краевой задачи![[Pasted image 20250617184055.png]]
	если ![[Pasted image 20250617184230.png]]
## Первая краевая задача в цилиндрической области для уравнения теплопроводности. Метод Галеркина
- (175) Функция $u(t,x) \in W^1_2(Ц_T)$ - обобщенное решение краевой задачи![[Pasted image 20250617184500.png]]
	если ![[Pasted image 20250617184542.png]]
## Гиперболические системы
- ![[Pasted image 20250617184638.png]]