# Numerical Methods
## Mathematical Analysis
Seatwork:
- SW #1

2023-08-12
### Numerical systems
Asst. Prof. Jonathan B. Cabero M,S

- Deals with numerical analysis on functions 
- Study of numerical algorithm use approximation for the problems of mathematical analysis 

Intermediate value theorem for continuous functions 
- Theorem Intermediate - value theorem for continuous functions 
- Let f(x) be continuous function on the interval [a,b]. If f(x) <= a <= f(x) for some number a and some x is an element [a,b]m then a = f(e) for some e element [a,b] 


Problem 1 

Find a real number x that is one has than its cube. Find tthe root of the function at 
$$ \in = 10^6 $$
Ex
	$$x = x^3-1 or -x -1 = 0$$
	Solve
		$$f(x) = x^3 -x-1 $$
		Evaluate 
			$$ f(x) at (1,2)$$


| x | 1.1 | 1.2 | **1.3** | **1.4** | 1.5|
| --- | --- | ---| ---|---|---|
| f(x) | -0.76 | -0.47 | **-0.61** | **0.34** | N\A|

| x | 1.31 | **1.32** | **1.33** | 1.34 | 1.35|
| --- | --- | ---| ---|---|---|
| f(x) | -0.6 | -0.2 | **0.2** | N\A | N\A|

| x | 1.321 | 1.322 | 1.323 | 1.324 | **1.325**|
| --- | --- | ---| ---|---|---|
| f(x) | N\A | N\A | N\A | N\A | **N\A**|

... **Keep going until it reaches 0 ** 
x = 1.3247

The mean value theorem 
- Similar to the intermediate value theorem 

Rolle's theorem 
- Let f(x) be continous on the interval [a,b] and differentiable on (a,b). If a f(a) = f(b) = 0, then f'(e) = 0, for some e element of (a,b)

 $$f(x) = x^3 - 4x ....at (-2,2)$$
 $$f(-2) = (-2)^3-4(-2) = 0$$
 $$ f(2) = 2^3-4(2) = 0  $$
 $$ f'(x) = 3x^2 - 4$$
 $$f'(c)=3c^2 - 4$$
 $$ f'(c) = 0 $$
 $$ 3c^2-4=0 $$
 $$\begin{align*} 3c^2&=4 \\ c^2&=\frac{4}{3} \\ c &= \pm \frac {2}{\sqrt{3}}\end{align*}$$

Mean value theorem for Derivatives 
- If f(x) is continous on the (closed and finite) interbal [a,b] and differentiable on (a,b) then 

Mean value theorem -- (f(b) - f(a))/(b-a)

$$ f(x) = x^3, (-2,2) $$
$$ f(-2) = 8'$$
$$f(2) = 8 $$
$$f(-2) \neq f(x)$$

$$\begin{align*} f'(x) = 3x^2 \\ f'(c) = 3c^2 \end{align*}$$
Apply mean value theorem
$$ \begin{align*} \frac {f(b) - f(a)}{b-a} \\ \frac {f(2) - f(-2)}{2-2} &= 3c^2 \\ \frac {8-(-8)}{4} &= 3c^2 \\ \frac {16}{4} &= 3c^2 \\ 3c^2 &=4 \\ c^2 &= \frac {4}{3} \\ c &= \pm \frac {2}{\sqrt 3} \end{align*}$$


Extreme value theorem 
- If f(x) is contionous on the close and finite interval [a,b], then c1, c2 e [a,b]  exist with f(c1) <= f(x) <= f(c2) for each x element of [a,b]. If f(x) is differentiable on (a,b) then the number c1 and c2 occur either t the endpoints of [a,b] or where f'(x) is zero. 

$$f(x) = \mathrm e^2 + 4x, (-2,2)$$
$$ \begin{align*} f'(x) &= \mathrm e^x - 4\\ f'(x) &=0 \\ \mathrm e ^2 - 4&=0 \\ \mathrm e^x&=4 \\ ln(\mathrm e^x &= 4)\\ x &= ln 4\end{align*} $$

2023-08-12
### Taylor's Formula with (Integral) Remainder
- if f(x) has n+1 continuous derivatives on [a,b], then for all x element of [a,b]


$$R_{n+1}(x)=\frac{1}{n!} \int_{c}^{x} (x-s)^n f^{(n+1)}(s)ds$$
#### Example 
1. $$\begin{align*} f(x)&=e^x, \; c=0 \\ f(x) &=e^x \;\; f(0)=1 \\ f'(x) &=e^x \;\; f'(0)=1 \\ f''(x) &=e^x \;\; f''(0)=1 \\ f'''(x) &=e^x \;\; f'''(0)=1 \end{align*}$$
$$e^x \approx 1 + x + \frac {x^2}{x!} + \frac {x^3}{3!}+...+\frac {x^n}{n!}+...$$

2. $$\begin{align*} f(x) &= ln\;x, \; &c = 12 \\ f(x) &=ln \;x, &f(1)=0 \\ f'(x) &= \frac {1}{x}=x^{-1} \; &f'(1)=1 \\ f''(x) &=-x^{-2} \; &f(1)=-1 \\ f'''(x)&=2x^{-3} \; &f'''(1) =2 \\ f''''(x) &=(-6x)^{-4} \; &f''''(1) =-6  \end{align*}$$


![[Pasted image 20230817144605.png]]
3. $$ f(x)= x^2e^n $$
   $$\begin{align*} x^2e^x \approx x^2(1+x+x^) x\end{align*}$$
### Taylor's theorem in terms of h 
- If f(x) possesses continuous derivatives of order 0,1,2
#### The Big O Notation 
$$\vartheta(h^{n+1}) = R_{n+1}(x)$$
$$\text{for some }\varepsilon \text{ let } x \text{ and } x+h $$
$$ \begin{align*} f(x+h) &= f(x) + f'(\varepsilon)h \\ f(x+h) &= f(x)+ \vartheta (h)\\ f(x+h) &=f(x) + f'^{(x)}h+ \frac{1}{2} f''(\varepsilon_2)h^2\\ f(x+h) &=f(x)+f'^{(x)}h + \vartheta (h^2) \\ f(x+h) &= f(x) + f'^{(x)}h + \frac {1}{2} f''^{(x)h^2} + \frac {1}{3} f'''(\epsilon_3)h^3 \\ f(x+h) &= f(x) + f'^{(x)}h + \frac {1}{2} f''^{(\epsilon_2)^{h^2}}+ \vartheta (h^3)\end{align*}$$
$$\text{and so on}$$


#### Example
Approximate 

a.) $$\sqrt{1.00001}$$
$$\text{Set } x =1, \; h=10^{-5}$$
$$ \begin{align*} f(x) &= \sqrt x = x^{\frac {1}{2}} \; &f(1)=1 \\ f'(x) &= \frac {1}{2}x^{-\frac {1}{2}} \; &f'(1)=\frac {1}{2} \\ f''(x) &= -\frac{1}{4}x^{-\frac {3}{2}} \; &f'(1)=\frac {1}{2} \\ f'''(x) &= \frac {3}{8}x^{- \frac {5}{2}} \; &f'''(1)=\frac {3}{8}\end{align*} $$
$$ \begin{align*} \sqrt{1.00001} &= \sqrt{1+10^{-5}}\\ & \approx 1+\frac {1}{2}h - \frac {1}{4}h^2 \\ &\approx 1+\frac {1}{2}(10^-3)-\frac {1}{4}(10^{-5})^2\\ &\approx 1.00000499999875 \end{align*} $$
b.) $$\sqrt {.99999}$$
$$\begin{align*} \sqrt {.99999} &= \sqrt{1-10^{-5}}\\ &\approx 1-\frac {1}{2}(10^-5) + \frac {1}{4}(10^{-5})^2\\ &\approx .99999999997875 \end{align*}$$


### Alternating Series Theorem

![[Pasted image 20230817145440.png]]
#### Examples 
![[Pasted image 20230817145616.png]]

![[Pasted image 20230817145636.png]]
![[Pasted image 20230817145705.png]]
![[Pasted image 20230817145724.png]]
![[Pasted image 20230817145747.png]]
![[Pasted image 20230817145809.png]]
![[Pasted image 20230817145820.png]]

### Fundamental Theorem of Algebra
![[Pasted image 20230817145906.png]]

#### Example 

$$ \begin{align*} P(x) &= 1+2x-3x^2 +4x^3-5x^4 \\ &= 1+x(2-3x+4x^2-5x^3) \\ &= 1+x(2-x(3-4x+5x^2)) \\ &= 1+x(2-x(3-x(4-5x)))\end{align*}$$
### Binomial Theorem 
![[Pasted image 20230817150138.png]]

#### Example 

![[Pasted image 20230817150611.png]]
$$\begin{align*}(x+y)^4 &= \binom{4}{0}x^4y^0 + \binom{4}{1}x^3y^1+\binom{4}{2}x^2y^2 + \binom{4}{3}x^1y^3+\binom{4}{4}x^0y^4 \\&=x^4+4x^3y+6x^2y^2+4xy^3+y^4\end{align*}$$
- **The triangle below the equation is the pascal triangle**

$$
\documentclass[preview,border=12pt]{standalone}

\usepackage{array}
\begin{document}
\begin{tabular}{>{$n=}l<{$\hspace{12pt}}*{13}{c}}
0 &&&&&&&1&&&&&&\\
1 &&&&&&1&&1&&&&&\\
2 &&&&&1&&2&&1&&&&\\
3 &&&&1&&3&&3&&1&&&\\
4 &&&1&&4&&6&&4&&1&&\\
5 &&1&&5&&10&&10&&5&&1&\\
6 &1&&6&&15&&20&&15&&6&&1
\end{tabular}
\end{document}
$$


