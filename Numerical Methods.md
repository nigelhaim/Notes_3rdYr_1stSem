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


![[Pasted image 20230817143739.png]]
#### Example 
![[Pasted image 20230817144005.png]]

![[Pasted image 20230817144421.png]]

![[Pasted image 20230817144605.png]]

### Taylor's theorem in terms of h 
- If f(x) possesses continuous derivatives of order 0,1,2
	![[Pasted image 20230817144705.png]]

![[Pasted image 20230817145349.png]]

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
- **The triangle below the equation is the pascal triangle**