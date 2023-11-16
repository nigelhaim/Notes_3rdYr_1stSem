	
## Mathematical Analysis
Seatwork:
- SW #1
- SW #2 
- SW #3
2023-08-12
### Numerical systems
Asst. Prof. Jonathan B. Cabero M,S

- Deals with numerical analysis on functions 
- Study of numerical algorithm use approximation for the problems of mathematical analysis 

## Intermediate value theorem for continuous functions 
- Theorem Intermediate - value theorem for continuous functions 
- Let f(x) be continuous function on the interval $[a,b]$. If f(x) <= a <= f(x) for some number a and some x is an element $[a,b]$ m then a = f(e) for some e element $[a,b]$


Problem 1 

Find a real number x that is one has than its cube. Find the root of the function at 
$$ \in = 10^6 $$
Ex
	$$x = x^3-1 \;or -x -1 = 0$$
	Solve
		$$f(x) = x^3 -x-1 $$
		Evaluate 
			$$ f(x) at (1,2)$$


****

|x=|1.1|1.2|**1.3**|**1.4**|1.5|
|---|---|---|---|---|---|
|$f(x)$|-0.769|-0.472|**-0.103**|**0.344**|0.875|


|x=|1.31|**1.32**|**1.33**|1.34|1.35|
|---|---|---|---|---|---|
|$f(x)$|-0.061909|**-0.020032**|**0.022637**|0.066104|0.110375|

|x=|1.321|1.322|1.323|**1.324**|**1.325**|1.326|
|---|---|---|---|---|---|---|
|$f(x)$|-0.015800839|-0.011561752|-0.007314733|**-0.003059776**|**0.001203125**|0.005473976|

|x=|1.3241|1.3242|1.3243|1.3244|1.3245|1.3246|**1.3247**|**1.3248**|1.3249|
|---|---|---|---|---|---|---|---|---|---|
|f(x)|-0.002633843479|-0.002207831512|-0.001781740093|-0.001355569216|-0.000929318875|-0.000502989064|**-0.000076579777**|**0.000349908992**|0.000776477249|

**x = 1.3247**

Solve

The mean value theorem 
- Similar to the intermediate value theorem 

### Rolle's theorem 
- Let f(x) be continous on the interval [a,b] and differentiable on (a,b). If a f(a) = f(b) = 0, then f'(e) = 0, for some e element of (a,b)

 $$f(x) = x^3 - 4x \; at \;(-2,2)$$
 $$f(-2) = (-2)^3-4(-2) = 0$$
 $$ f(2) = 2^3-4(2) = 0  $$
 $$ f'(x) = 3x^2 - 4$$
 $$f'(c)=3c^2 - 4$$
 $$ f'(c) = 0 $$
 $$ 3c^2-4=0 $$
 $$\begin{align*} 3c^2&=4 \\ c^2&=\frac{4}{3} \\ c &= \pm \frac {2}{\sqrt{3}}\end{align*}$$

### Mean value theorem for Derivatives 
- If f(x) is continuous on the (closed and finite) interval [a,b] and differentiable on (a,b) then 

$$Mean \; Value \; Theorem = \frac {f(b)-f(a)}{b-a}$$

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
## Taylor's Formula with (Integral) Remainder
- if f(x) has n+1 continuous derivatives on [a,b], then for all x element of [a,b]


$$R_{n+1}(x)=\frac{1}{n!} \int_{c}^{x} (x-s)^n f^{(n+1)}(s)ds$$
#### Example 
1. $$\begin{align*} f(x)&=e^x, \; c=0 \\ f(x) &=e^x \;\; f(0)=1 \\ f'(x) &=e^x \;\; f'(0)=1 \\ f''(x) &=e^x \;\; f''(0)=1 \\ f'''(x) &=e^x \;\; f'''(0)=1 \end{align*}$$
$$e^x \approx 1 + x + \frac {x^2}{x!} + \frac {x^3}{3!}+...+\frac {x^n}{n!}+...$$

2. $$\begin{align*} f(x) &= ln\;x, \; &c = 12 \\ f(x) &=ln \;x, &f(1)=0 \\ f'(x) &= \frac {1}{x}=x^{-1} \; &f'(1)=1 \\ f''(x) &=-x^{-2} \; &f(1)=-1 \\ f'''(x)&=2x^{-3} \; &f'''(1) =2 \\ f''''(x) &=(-6x)^{-4} \; &f''''(1) =-6  \end{align*}$$
3. $$ \begin{align*}&f(x)= x^2e^n \\ &x^2e^n \approx x^2(1+x+\frac {x^2}{2!} + \frac {x^3}{3!} + \frac {x^4}{4!} + ....)\\ &\text{  }\approx x^2+x^3+\frac {x^4}{2} + \frac {x^5}{6} + \frac{x^6}{24} + ..... \end{align*}$$
   $$\begin{align*} x^2e^x \approx x^2(1+x+x^) x\end{align*}$$
## Taylor's theorem in terms of h 
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


## Alternating Series Theorem

$$\begin{align*} &\text{If } a_1 \geq a_2 \geq ... \geq a_n...0 \text{for all n in } \lim_{n \to n} a_n = 0,\\ &\text{then the alternating series} \end{align*}$$
$$a_1 - a_2 + a_3 - a_4 + ...$$
$$\text{converges, that is}$$
$$\lim_{n \to \infty} \sum\limits_{k=1}^n (-1)^{k-1}a_k=\lim_{n\rightarrow\infty}\sum^n_{k=1}(-1)^{k-1}a_k=\lim_{n\rightarrow\infty}S_n=S$$

$$\text{Where S is its sum and } S_n \text{ is the nth partial sum. Moreover, for all n}$$
$$|S-S_n| \leq a_{n+1}$$
$\text{Where S is its sum and } S_n \text{is the nth partial sum. Moreover, for all } n|S-S_n|\leq a_{n+1}$
Convergent Series 
A series is convergent ifi the sequence of its partial sums ${S_1,S_2,S-3...}$ converges; in other words, it approaches a given number. In more formal language, a series converges if there exists a limit $\iota$ such that for any arbitrarily small positive number $\epsilon > 0$, there is a large integer $N$ such that for all $n \geq N$,
$$|S_n - \iota| \leq \epsilon$$
Any series that is not convergent is said to be divergent

#### Examples 
1. The reciprocals of the positive integers produce a divergent series (harmonic series):
	$\frac{1}{1}+\frac{1}{2}+\frac{1}{3}+\frac{1}{4}+\frac{1}{5}+\frac{1}{6}+...\to\infty$
2. Alternating the signs of the reciprocals of positive integers produces a convergent series: 
	$\frac{1}{1}-\frac{1}{2}+\frac{1}{3}-\frac{1}{4}+\frac{1}{5}...=ln(2)$
3. Alternating the signs of the reciprocals of positive odd integers produces a convergent series (the Lebniz formula of pi):
	$\frac{1}{1}-\frac{1}{3}+\frac{1}{5}-\frac{1}{7}+\frac{1}{9}-\frac{1}{11}+...=\frac{\pi}{4}$
	
4. The reciprocals of prime numbers produce a divergent series (so the set of primes is "large"):
	$\frac{1}{2}+\frac{1}{3}+\frac{1}{5}+\frac{1}{7}+\frac{1}{11}+\frac{1}{13}+...\to \infty$
5. The reciprocals of triangular numbers produce a convergent series:
	$\frac{1}{1}+\frac{1}{3}+\frac{1}{6}+\frac{1}{10}+\frac{1}{15}+\frac{1}{21}+...=2$
	
6. The reciprocals of factorials produce a convergent series (see e):
	$\frac{1}{1}+\frac{1}{1}+\frac{1}{2}+\frac{1}{6}+\frac{1}{24}+\frac{1}{120}+...=e$
7. The reciprocals of square numbers produce a convergent series (the Basel problem):
	$\frac{1}{1}+\frac{1}{4}+\frac{1}{9}+\frac{1}{16}+\frac{1}{25}+\frac{1}{36}+...=\frac{\pi^2}{6}$
	
8. The reciprocals of powers of 2 produce a convergent series (so the set of powers of 2 is "small"):
	$\frac{1}{1}+\frac{1}{2}+\frac{1}{4}+\frac{1}{8}+\frac{1}{16}+\frac{1}{32}+...=2$
9. Alternating the signs of reciprocals of powers of 2 also produces a convergent series:
	$\frac{1}{1}-\frac{1}{2}+\frac{1}{4}-\frac{1}{8}+\frac{1}{16}-\frac{1}{32}+...=\frac{2}{3}$
10. the reciprocals of the Fibonacci numbers produces a convergent series (see $\psi$)
		$\frac{1}{1}+\frac{1}{2}+\frac{1}{3}+\frac{1}{5}+\frac{1}{8}+...=\psi$

### Fundamental Theorem of Algebra
If $p(x)$ is a polynomial of degree $n \geq 1$, that is,
$p(x) = a_0 + a_1x +a_2 x^2+...+a_xx^n$

with $a_0,a_1,a_2,...,a_n$ real or complex numbers and $a_n \neq 0$. Then $p(x)$ has at least one zero, that ism there exists a complex number $\epsilon$ such that $p(\epsilon) = 0$.

The polynomial $p(x)$ can be written 
$p(x) = \sum\limits_{i=0}^n a_ix^i = \sum\limits_{i=0}^n(a_i\prod\limits_{j=1}^ix)$
To evaluate a polynomial $p(x)$ efficiently, write
$p(x) = a_0 + a_1x+a_2x^2+...a_nx^n$
In the form 
$p(x)=a_0+x(a_1+x(a_2+...+x(x_{n-1}+x(a_n)))...))$

#### Example 

$$ \begin{align*} P(x) &= 1+2x-3x^2 +4x^3-5x^4 \\ &= 1+x(2-3x+4x^2-5x^3) \\ &= 1+x(2-x(3-4x+5x^2)) \\ &= 1+x(2-x(3-x(4-5x)))\end{align*}$$
### Binomial Theorem 

The binomial theorem is defined by
$(a+b)^n = \binom{n}{0}a^nb^0+\binom{n}{1}a^{n-1}b^1+...+\binom{n}{n-1}a^1b^n-1+\binom{n}{n}a^0b^n$

Where the binomial coefficient is $\binom{n}{r} = \frac {n!}{r!(n-r)!}$
The (r+1)th term is $\binom{n}{r}a^{n-r}b^r$

#### Example 


$$\begin{align*}(x+y)^4 &= \binom{4}{0}x^4y^0 + \binom{4}{1}x^3y^1+\binom{4}{2}x^2y^2 + \binom{4}{3}x^1y^3+\binom{4}{4}x^0y^4 \\&=x^4+4x^3y+6x^2y^2+4xy^3+y^4\end{align*}$$
- **The triangle below the equation is the pascal triangle**



2023-08-19

## Error
- Numerical methods deal with approximation, since its approximation it is prone to error.

2 sources of errors
- Rounding off errors
	- deals Significant digits
		- Takes a meaning that contributes to its accuracy 
		- often used in connection with rounding
		- A more general purpose technique than rounding to n decimal place
- Truncation error

#### Rules 
1. All non-zero digits are considered significant 
2. Zeros appearing anywhere between two non-zero digits are significant 
3. Leading zeros are not significant 
4.  Trailing zeros in a number containing a decimal point are significant 
5. The number 0 has one significant digits
6. The significance of trailing zeros in a number not containing a decimal point can be indefinite. Thus, the following conditions are given:
	1. A bar may be placed over the last significant figure, any trailing zeros following this are not significant 
	2. The last significant digit of a number maybe underlined
	3. A decimal point may be placed after the number 
Note: in the combination of a number and a unit of measurement, we can easily determine the significant digit by supplying the suitable unit prefix


#### Examples 

|  |  |  |
| --- | --- | --- |
| 2.745 | has four significant digits: | 2,7,4,5 |
| 20.003 | has five significant digits:  | 2,0,0,0,3 |
| 0.0021 | has two significant digits: | 2,1 |
| 0.002100 | has four significant digits: | 2,1,0,0 |
| 20000 | has three significant digits| 2,0,0|
|0.201000| has five significant digits | 2,0,1,0,0 |
|1.05 $10^5$| has three significant digits:  |1,0,5|
|2.0300 $10^7$| has five significant digits: |2,0,3,0,0|


### Measuring errors
**Error** - normally encountered during the calculation in the numerical analysis

To deal errors considering the following factors
1. Identification where the error comes from
2. Quantifying the error 
3. Minimizing the error as per the needs 

### Sources of error 
- Error can arise due to several factors
1. May be in the modelling technique 
2. May arise from mistakes in programs themselves 
3. May arise from mistakes in the measurement of physical quantities

**Round off error**
- Occur because digital computers cannot represent some quantities exactly its value can be calculated by deviating the rounded digits and the exact value. 
- Two component of round off error involved in numerical calculations:
	- Digital computers have size and precision limits on their ability to represent the numbers
	- Certain numerical manipulation are highly sensitive to round off errors.

**Truncation error**
- Caused by truncating a mathematical procedure. That is, replacing an infinite process by a finite one. 
- Its value can also be calculated by getting the deviation between the exact vale and its approximate value
#### Examples 
$$\epsilon = 10^4$$
$$e^{0.5} \approx 1.648721  $$
$$e^x \approx 1+x+ \frac{x^2}{2}+ \frac{x^3}{3!}+\frac{x^4}{4!}+\frac{x^5}{5!}+$$
$$n=5$$


$$ \begin{align*}e^0.5 &\approx 1 + 0.5 + \frac {.5^2}{2} +\frac {.5^3}{3!}+ \frac {.5^4}{4!}+\frac {.5^5}{5!} \\ &\approx 1.6487 \end{align*}$$
$$n=4$$
$$\begin{align*} e^.5 &\approx 1+0.5 + \frac{.5^2}{2!} +\frac{.5^3}{3!} +\frac{.5^4}{4!} \\ &\approx 1.6484\end{align*}$$


$$\text{The rounding off error is} $$
$$e^{.5} - 1.648721$$

$$\text{The Truncating error is} $$
$n=2$
$$e^x-1+x+\frac{x^2}{2} = \frac{x^3}{3!}+ \frac{x^4}{4!}+\frac{x^5}{5!}+...+\frac{x^n}{n!}+.+R_{n+1}$$


#### True error and Relative error
- One of the most common error that we encountered during numerical calculation is the true error which is  just the deviation between the true or exact value and the approximate value, i.e,

$$TrueError = TrueValue - ApproximateValue $$

The relative true error which is the ratio between the true error and the true value, i.e,

$$RelativeError = \frac{TrueError}{TrueValue}$$
#### Example

$$\begin{align*}f(x)=\sqrt{x}=x^{\frac{1}{2}}  \;\;,x=5 \end{align*}$$
$$f'(x)=\frac {1}{2}x^{-\frac{1}{2}} = \frac{1}{2\sqrt{x}}$$
$$f'(x) = \frac {1}{2\sqrt{5}}=$$
$$f'(x)= \lim_{h \to 0}\frac{f(x+h)-f(x)}{h}$$
$$f'(x)\approx \frac{f(x+h)-f(x)}{h}, \;\; h=0.01, \;\; x=5$$

$$\text{The true error is}$$
$$f'(5) \approx \frac{\sqrt{5.01}-\sqrt{5}}{.01}\approx$$


$$Absolute \; Error = |\frac {1}{2\sqrt{5}} - \frac{\sqrt{5.01}-\sqrt{5}}{.01}|$$
$$Relative \; Error = \frac {|\frac{1}{2\sqrt{5}}-\frac{\sqrt{5.01}-\sqrt{5}}{0.1}|}{\frac{1}{2\sqrt{5}}}$$


#### Approximate error 
- Calculated only if true values are known
- Useful if a program is in working order 
- When solving a problem numerically, we will only have access to approximate values 
	- Approximate error is defined as the deviation between the present approximation and previous approximation, i.e,
	- $\text{Approximate Error = Present Approximation - Previous Approximation}$

#### Example
This is connected to the previous example 
$$h=0.001$$
$$f'(5)\approx \frac{\sqrt{5.001}-\sqrt{5}}{0.001}$$
$$Approx \; Error = |\frac{\sqrt{5.001}-\sqrt{5}}{0.001} - \frac{\sqrt{5.01}-\sqrt{5}}{0.01}|$$

#### Relative Approximate Error 
- Defined as the ratio between the approximate error and the present approximation 
$$RelativeApproximateError = \frac{Approximate \; Error}{Present \; Approximation}$$
##### Example 
This is also Connected to the previous example
$$Relative \; Approx \; Error = \frac {Approx \; Error}{\frac {\sqrt{5.001}-\sqrt{5}}{0.001}}$$

#### Tolerance 
- We can use the approximate error to minimize the error when solving mathematical model using numerical methods by calculating the relative approximate error at the end of every iteration 
- We can pre-specify a minimum acceptable tolerance called the pre-specified tolerance
- If the value of absolute relative approximate error is at the most pre-specified tolerance then the acceptable error has been reached and no more iteration would be needed. Otherwise, one may pre-specify how many significant digits they would like to be correct in the answer
- If one wants at least significant digits to be correct in the answer, the you would need to have the absolute relative approximate error.

## Number Representation 
### Octal and Hexadecimal representation 
- First Year and 2nd Year topics 

### Binary system
- In the binary system the base is 2, the integer coefficients may take the vlaues 0 or 1 
### Normalized Floating-point Representation 
Every nonzero real number x has a floating-point representation
$$x=\pm M x r^e, where \frac{1}{r} \leq M < 1 \; or -\frac{1}{r} \leq M < -1$$
$$Where$$
$$M = \sum_{k=1}^t d_kr^{-k}$$
M is called the mantissa, e is an integer called exponent, r the base, $d_k$ is the value of the kth digit


#### Examples 

13th picture 

$-18.25 \text{ has representation } -0.1825 * 10^2(M - 0.1825, e =2)$
$0.1 has \; representation \; 0.1*10^0(M=0.1,e=0)$ 
$\frac {1}{15} \; has \; representation (\frac{1}{15}*10)*10^{-1}(M=0.66, e=-1)$

### Machine numbers 
- A Machine number for a calculator is a real number that it stores exactly normalized floating-point form. 
- A nonzero x is a machine number if and only if its normalized floating decimal point representation is of the form 
$$x\pm M*10^e$$
- Computers use a normalized floating point binary representation for real numbers
$$x \pm M * 2^e$$

#### Example 

$-18.25 \; has \; representation \; -(\frac{73}{4}*\frac{1}{32})*2^5(M=\frac{73}{128'},e=5)$
$0.1  \; has \; representation \;  (\frac{1}{10}*8)*2^{-3}(M-\frac{4}{5}e=-3)$
$\frac{1}{15}  \; has \; representation \; (\frac{1}{15}*8)*2^{-3}(M=\frac{8}{15},e=-3)$


### Decimal System 
- The base of the decimal system is 10. The digits 0,1,2,3,4,5,6,7,8,9. A string of represents a number according to the formula 


2023-08-24

## Solution of Equation 
**Iterative method**
- The solution of a problem by successive approximation is often the simplest method
- A machine will shifty and accurately carry out routine calculations repeated over and over again until an answer of sufficient accuracy is obtained

Example 
1. Find $\sqrt{8}$ by iteration , $\epsilon = 10^6$
Solution: 
$$\sqrt{8} = 2.828427$$
$$\begin{align*} \frac{8}{3} &= 2.666667 \\ \frac{3+2.6666667}{2} &= 2.8333333 \\ \frac{8}{2.83333333} &= 2.823529 \\ \frac{2.8333333+2.823529}{2} &= 2.828430 \\ \frac{8}{2.828430} &= 2.828424\end{align*}$$

	 
Iteration formula of the square root of a certain number 
$$x_{k+1} = \frac{1}{2}(x_k + \frac{n}{x_k})$$

2. Find the fraction representation near 0.234567 , $\epsilon = 10^{-6}$
Solution:
$$\frac{1+1}{5+4} = \frac{2}{9} = 0.22222 \downarrow$$
$$\frac{1+2}{4+9}= \frac{3}{13}=.230777\downarrow$$
$$\frac{1+3}{4+13} = \frac{4}{17} = 0.235294\uparrow$$
$$\frac{4+3}{17+13} = \frac{7}{30} = .2333333\downarrow$$
$$\frac{7+4}{30+17} = \frac{11}{47} = 0.234042\downarrow$$
$$\frac{11+4}{47+17} = \frac{15}{64} = 0.234375\downarrow$$
$$\frac{15+4}{64+17} = \frac{19}{81} = 0.234567\uparrow$$


2023-08-26

## Solution of Equation 
**Iteration method**
- The simplest method
- A machine will shiftly and accurately carry out routine calculations repeated over and over again until a sufficient answer occur 

### Fixed-point Method
if  is a continuous function on the interval [a,b] for all $x \epsilon [a,b]$, then $g(x)$ has fixed point in [a,b]. Suppose in addition, that $g'(x)$ exist on (a,b), and a positive constant $k<1$ exists with $|g'(x)|\le k <1$ for all $x\epsilon (a,b)$. Then the fixed point in [a,b] is unique.


### Iteration method
**Procedures**

1. Choose an initial approximation $x_0$ such that $x_0 \epsilon [a,b]$ ( The numbers inside your brackets are limits)
2. Choose a convergence parameter $\epsilon > 0$
3. Compute a new approximation $z_{new}$ using iterative formula 
4. check if $|x_{new} -x_0|<\epsilon then x_{new}$ is the desired approximation root; otherwise set $x_0=x_{new}$ and go to step 3


### To approximate the fixed point 
- To approximate the fixed point of a function g, we choose an initial approximation $p_0$ and generate the sequence ${p_n}^{\infty}_{n=0}$ by letting $p_n =g(p_{n-1})$ for each $n\geq1$. If the sequence converges to p and g is continuous, then 
- $p = \lim_{n\to \infty}p_n=\lim_{n\to \infty}g(p_{n-1})=(\lim_{n\to \infty}p_{n-1}) =g(p)$


### Graph 

pic 4


#### Example 
$$x^2 + x-1$$
$$\begin{align*}x^2+x&=1\\x(x+1)&=1\\x_{n+1}&=\frac{1}{x_{n}+1}\end{align*}$$

Pick and miss (sir Cabero)

##### 2 Roots of quadratic formula 
**Quadratic formula**  - $x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}$

The derivative of quadratic formula 

$\begin{align*}x_1+x_2 &= -\frac{b+\sqrt{b^2-4ac}}{2a} + \frac{-b-\sqrt{b^2-4ac}}{2a}\\&=-\frac{2b}{2a} = -\frac{b}{a}\end{align*}$


#### Example 

The equation $x^3+4x^2-10=0$ has a unique root in [1,2]

for example, 

Solution: Change the equation in the form $x_{n+1} = g(x_n)$ by simple algebraic manipulation 
| $\begin{align*}4X^2&=10-x^3\\x^3+4x^2&=10\end{align*}$ | $\begin{align*}x^2&=\frac{1}{4}(10-x^3)\\x^2(x+4)&=10\end{align*}$ | $\begin{align*}x&=\frac{1}{2}(10-x^3)^{\frac{1}{2}}\\ x&=(\frac{10}{x+4})^{\frac{1}{2}}\end{align*}$ |
| --- | --- | --- |
| $Let x_0=\frac{1}{2}(1+2)=1.5$ | | |




### Bisection method 
- Suppose $f(x)$ is a continuous function defined on the interval [a,b] with $f(a)$ and $f(b)$ of opposite signs. Using the Intermediate Value Theorem, there exist p in [a,b] with $f(p)=0$. Although the procedure will work for the case when $f(a)$ and $f(b)$ have opposite signs and there is more than one root in the interval (a,b) we assume that the root in this interval is unique. The method calls for a repeated halving of sub-intervals of [a,b] and at each step, locating the half containing p. 

#### Steps 
- set $a_1 = a\; and \; b_1=b$ and let $p_1$ be the midpoint of [a,b] that is
$$p = \frac{1}{2} (a+b)$$
- If $f(p)=0$, then p as $p_1$. If not then $f(p_1)$ has the same sign as either $f(a_1)$ or $f(b_1)$. If $f(p_1)$ and $f(a_1)$ have the same sign, then $p\epsilon(p_1,b_1)$ and we set $a_2 = p_1$ and $p_2 = b_1$. If $f(p_1)$ and $f_(a_1)$ have the opposite signs then $p\epsilon(a_1, b_1)$ and set $a_2=a_1$ and $b_2=p_1$. We then reapply the process to the interval [a,b].
#### Procedures for Bisection Method 
1. Establish and interval $a \leq x \leq b$ such that $f(a)$ and $f(b)$ are of opposite sign; that is $f(a)*f(b) < 0$ 
2. Choose an error tolerance $(\epsilon>0)$ value for the function 
3. Compute a new approximation for the root
$$c_n = \frac{(a_n+b_n)}{2}, n=1,2,3,...$$
4. Check the tolerance. If $|f(c_n)|\leq \epsilon$, then use $c_n(n=1,2,3,...)$ for the desired root; otherwise continue.
5. Check if $f(a_n) *f(c_n)<0$, then set $b_n=c_n$; otherwise, set $a_n=c_n$
6. Go back to step 3 and repeat the process

#### The Newton-Raphson (Newton's) Method

- Suppose that $f$ is continuous on the interval [a.b]. Let $x \epsilon [a,b]$ be an approximation that $f(x) \neq 0 and [x-p]$ is small. Consider the first Taylor's polynomial for $f(x)$ expanded about $x$.
- $f(x)=f(\bar{x})+(x-\bar{x})f'(\bar{x})+\frac{(x-\bar{x})^2}{2!}f''(\epsilon(x))$
- where $\epsilon(x)$ lies between $\bar{x}$ and $x$. Since $f(p)=0$, this equation with $x=p$ gives d
$$0=f(\bar{x})+(p-\bar{x})f'(x)+\frac{(p-\bar{x})^2}{2!}f''(\epsilon(p))$$
- Newton's method is derived by assuming that, since $|\bar{x}-p|$ is small. the term involving $(p-\bar{x})^2$ is negligible and that 
$$0 \approx \bar{x} - \frac{f(\bar{x})}{f'(x)}$$
- This set the stage for the Newton-Raphson method, which starts with an initial approximation $p_0$ and generates the sequence {$p_n$} defined by 
$$p_n = p_{n-1} - \frac{f(p_{n-1})}{f'(p_{n-1})}$$


Starting with the initial approximation the approximation $p_0$, the approximation $p_1$ is the x-intercept of the tangent lint to the graph of f at $(p_0, f(p_0))$. The approximation $p_2$ is the x-intercept fo the tangent line to the graph of f at $(p_1, f(p_1))$, and so on.

Example 

To obtain the unique solution to $x^3+4x^2-10=0$ on the interval [1,2] by Newton's Method, generates the sequence ${p_n}^\infty_{n=0}$ by
$p_n = p_{n-1}-\frac{p^3_{n-1}+4p^2_{n-1}-10}{3p^2_{n-1}+8p_{n-1}}$

$$f(x)=x^3-4x^2-10$$
$$f'(x) = 3x^3-8x$$


$$p_1 = p_{0}-\frac{p^3_{0}+4p^2_{0}-10}{3p^2_{0}+8p_{0}}$$
$$p_2 = p_{2-1}-\frac{p^3_{2-1}+4p^2_{2-1}-10}{3p^2_{2-1}+8p_{2-1}}$$

#### Procedures of the Newton's Method 
1. Find the initial approximation $x_0$ for the root by sketching the graph of the function 
2. Evaluate the function $f(x)$ and the derivative $f'(x)$ at the initial approximation 
3. Check if $f(x_0)=0$ then $x_0$ is the desired approximation to a root. But if $f'(x_0)=0$, then go back to step 1 to choose a new approximation 
4. Establish the tolerance $(\epsilon>0)$ value for the function
5. Compute a new approximation for hte root using iterative formula
6. Check the tolerance. If $|f(x_n)|\leq\epsilon$, for $n\geq0$, then end; otherwise go back to step 4 and repeat the process. 

#### Secant Method 
- Starting with two initial approximations with two initial approximations $p_0$ and $p_1$, the approximation $p_2$ is the x - intercept of the line joining ($p_0,f(p_0)$) and $(p_1,f(p_1))$. The approximation $p_3$ is the x-intercept of the line joining $(p_1,f(p_1))$ and $(p_2,f(p_2))$ and so on.
- With two initial approximations $p_0$ and $p_1$ generates the sequence {$p_n$} defined by 
$$p_n = p_{n-1} - \frac{f(p_{n-1})(p_{n-1}-p_{n-2})}{f(p_{n-1})-f(p_{n-2})}$$

**Procedures of Secant method**
- Choose the two initial approximations $x_0$ and $x_1$
- Check if $f(x_0)=f(x_1)$, go to step 1; otherwise; continue 
- Establish the tolerance ($\epsilon>0$) value for the function
- Compute a new approximation for the root using iterative formula 
- Check the tolerance. If $|x_n-x_{n-1}| \leq \epsilon, \; for \;n\geq1$, then end; otherwise go back to step 4 and repeat the process  



2023 - 09 - 14

# LT #1. CS 26110 
1. Find all number c that satisfy the conclusion of Rolle's Theorem/Mean Value theorem on the following functions:
1.1 $f(x)=\frac{x}{x+4},\;[0.4]$
	Ans. $f(0) -0,f(4)=\frac{1}{2}$

$$f'(x)=\frac{(x+4)(1)-x(1)}{(x+4)^2}=\frac{4}{(x+4)^2}$$
$$f'(c)=\frac{4}{(c+4)^2}=\frac{\frac{1}{2}-0}{4-0}=\frac{1}{8}$$
$$\begin{align*} \frac{4}{(c+4)^2} &= \frac{1}{8}\\ 4 &= \frac{(c+4)^2}{8}\\32&=(c+4)^2 \\ \sqrt{32} &= c+4 \end{align*}$$
$$c=\sqrt{32}-4$$

1.2 $f(x)=x\sqrt{x+4},\;[-4,0]$
Ans. $f(-4)=0,\;f(0)=0$
$$f'(x)=(1)\sqrt{x+4}+x(\frac{1}{2})(x+4)^{\frac{1}{2}}$$
$$f'(c)=\sqrt{c+4}+(\frac{c}{2\sqrt{c+4}})=0$$
$$\frac{2(c+4)+c}{2\sqrt{c+4}a}=0$$
$$3c=-4$$
$$c=-\frac{4}{3}$$

2. Find the Fifth degree Taylor polynomial $P_5(x) use it to approximate \epsilon = 10^{-8}$
2.1 $\sqrt{1.002}$
Ans.
$$\begin{align*}f(x)&=x^{\frac{1}{2}}\\f'(x)&=\frac{1}{2}x^{-\frac{1}{2}}\\f''(x)&=-\frac{1}{4}x^{-\frac{3}{2}}\\f'''(x)&=\frac{3}{8}x^{-\frac{5}{2}}\\f^{(IV)}(x)&=-\frac{15}{16}x^{-\frac{5}{2}}\\\end{align*}$$
$$x=1,\;h=.002$$
$$\sqrt{1.002}\approx1+(\frac{1}{2})(.002)-(\frac{1}{4})(.002)^2+(\frac{3}{8}(.002)^3-(\frac{15}{16})(.002)^4$$
$$\approx 1.00099950$$
3. Convert the following 
3.1 Convert $(0.1100011)_2$ to decimal form in fraction form 
- **Ans. 99/128**
3.2 The first five binary digits of $(0.1)_{10}$
- **Ans. $(.00011)_2$**
3.3 The decimal floating point form of $\frac{2}{125}$
- **Ans. $0.16*10^{-1}$**
4. Solve the root of $f(x)=e^x-2-x$ on the interval [-2.4, -1.6] accurate to $10^{-4}$ using the bisection method 
- **Ans -1.8414**

|n|a|b|pn|f(pn)|f(a)|$f(a)*f(pn)$|
|---|---|---|---|---|---|---|
|1|-2.4000|-1.6000|-2.0000|0.1353|0.4907|0.0664|
|2|-2.0000|-1.6000|-1.8000|-0.0347|0.1353|-0.0047|
|3|-2.0000|-1.8000|-1.9000|0.0496|0.1353|0.0067|
|4|-1.9000|-1.8000|-1.8500|0.0072|0.0496|0.0004|
|5|-1.8500|-1.8000|-1.8250|-0.0138|0.0072|-0.0001|
|6|-1.8500|-1.8250|-1.8375|-0.0033|0.0072|0.0000|
|7|-1.8500|-1.8375|-1.8438|0.0020|0.0072|0.0000|
|8|-1.8438|-1.8375|-1.8406|-0.0007|0.0020|0.0000|
|9|-1.8438|-1.8406|-1.8422|0.0007|0.0020|0.0000|
|10|-1.8422|-1.8406|**-1.8414**|0.0000|0.0007|0.0000|
5. Solve the equation $e^{-x}-x=0$ using the secant method, starting at $x_0=0$ and $x_1=1$, accurate to $10^{-4}$
- **Ans 0.6571**

|n|xn-1|xn|f(xn-1)|f(xn)|xi+1|f(xi+1)|
|---|---|---|---|---|---|---|
|1|0.0000|1.0000|1.0000|-0.6321|0.6127|-0.0708|
|2|1.0000|0.6127|-0.6321|-0.0708|0.6383|-0.1101|
|3|0.6127|0.6383|-0.0708|-0.1101|0.6344|-0.1042|
|4|0.6383|0.6344|-0.1101|-0.1042|0.6350|-0.1050|
|5|0.6344|0.6350|-0.1042|-0.1050|0.6349|-0.1049|
|6|0.6350|0.6349|-0.1050|-0.1049|0.6349|-0.1049|
|7|0.6349|0.6349|-0.1049|-0.1049|0.6349|-0.1049|
## Calculus of Finite Differences 
**Finite difference operators**

The calcualus of infinite difference is important in the theory of interpolation and numerical differentiation and integration. Some of elementary procedures of the calculus of finite difference will be considered. It is desirable to have fmailiarity with them, since finite differences also occurs in curve fitting, smoothing of data and solving differential equations by approximate numerical methods.

#### Fundamental Operators of the Calculus of Finite Difference 

The calculus of finite differences is facilitated by the use of certain operators. An operator may be defined as symbol placed before a function to indicate the application of some process to the function to produce a new function. 

| Operator | | |
|---|---|---|
|Shifting operator | $Ef(x)=f(x+h)$ | (3.1)|
|Forward or Advancing Difference operator | $\Delta f(x)=f(x+h)-f(x)$ | (3.2) |
|Bakcward or Regressing Difference Operator | $\nabla f(x)=f(x+\frac{1}{2}h)-f(x-\frac{1}{2}h)$|(3.3)|
|Central Difference Operator  | $\delta f(x)=f(x+\frac{1}{2}h)-f(x-\frac{1}{2}h)$|(3.4)|
|Averaging Operator | $\mu f(x)=\frac{1}{2}[f(x+\frac{h}{2})+f(x-\frac{h}{2})]$|(3.5)|
|Derivative Operator | $Df(x)=\frac{d}{dx}f(x)=f'(x)$| (3.6)|
|Anti-Derivative Operator | $D^{-1}=\int f(x)dx+C$|(3.7)|
|Constant Operator | $kf(x)=kf(x)$|(3.8)|
|Summation Operator | $\sum f(x)=\Delta^{-1}f(x)$|(3.9)|
|Anti-Difference Operator |$\Delta^{-1}f(x)=\frac{1}{\Delta}f(x)$|(3.10)|
where h is the interval

The shifting operator $E$ when applied to a function means that that function to be replaced by its value h units to the right, $D$ indicates differentiation, and the constatn operator k merely multiples the function by a given constant 

If an operator is applied to a function and a second operator is applied to a resting function, these operators are written as a product. for Example 

$$\Delta f(x)=\Delta f'(x)=f'(x+h)-f'(x)=D\Delta f(x)$$
Product of powers of operators combine according to the law of exponents, that is 
$$\Delta ^3\Delta^2f(x)=\Delta^5f(x)$$
We restrict the powers of D and $\Delta$ to be integral and nonnegative numbers. However, all real number power of E may be allowed.
$$E^n f(x)=f(x+nh)$$
Also 
$$E^mE^nf(x)=E^{m+n}f(x)=f(x+mh+nh)$$
The sum or difference of two operators applied to a function is defined to be the sum or difference of the functions resulting form the application of each operator; that is 
$$E\pm\Delta)f(x)\pm\Delta f(x)$$
These operators may be combined as if they are algebraic quantities procided they conform to the following Laws of Algebra 

$$\begin{align*}A+B&=B+A\\A+(B+C)&=(A+B)+C\\AB&=BA\\A(BC)&=(AB)C\\A(B+C)&=AB+AC\end{align*}$$
For example
1. $E^mDf(x)=DE^mf(x)$
$$E^mDf(x)=E^mf'^{(x)}=f'(x+mh)$$
2. $(D^{\frac{1}{2}}\Delta-D)(E^{1}{2}\Delta+D)=E\Delta^2-D^2$
3. $(D-E)^2=D^2-2DE+E^2$
Two operators with the property that when they are applied to the same function they yield the same result are said to be operationally equivalent. Now from the definition of $\Delta f(x)$, we have 

| | | |
|---|---|---|
||$\Delta f(x)=f(x+h)-f(x)=Ef(x)-f(x)$|(3.11)|
||or $\Delta f(x)=(E-1)f(x)$|(3.12)|

So we have the operational equivalences 

| | | |
|---|---|---|
||$\Delta = E - 1$|(3.13)|
| | $E=1+\Delta$ | (3.14)|
||$1=E=\Delta$|(3.15)|
||$\Delta f(x)=\delta f(x+\frac{h}{2})=\delta E^{\frac{1}{2}}f(x)$|(3.16)|
||$\Delta = \delta E^{\frac{1}{2}}$|(3.17)|
| |$\delta = \Delta E^{-\frac{1}{2}}$|(3.18)|
||$\delta = E^{\frac{1}{2}}-E^{-\frac{1}{2}}$|(3.19)|

## Factorial Polynomial 
- The Factorial polynomial is defined by: 
$$(x)^{(n)}=x(x-1)(x-2)...(x-n+1)$$

$$and$$
$$(x)^{-(n)}= \frac{1}{(x+1)(x+2)...(x+n)}$$

#### Exmples 
1. $x^{(4)}=x(x-1))(x-2)(x-3)$
2. $x^{(-4)}=\frac{1}{(x+1)(x+2)(x+3)(x+4)}$
3. $(x- 5)^{(-3)}=(x+5)(x+4)(x+3)$
4. $(x-5)^{(-3)} = \frac{1}{(x-4)(x-3)(x-2)}$
5. $\begin{align*}(x+6)(x+7)(x+8)(x+11)&=(x+6)(x+7)(x+8)(x+9+2)\\&=(x+6)(x+7)(x+8)(x+9)+2(x+6)(x+7)(x+8)\\&=(x+9)^{(4)}+2(x+8)^{(3)}\end{align*}$
6. $\begin{align*}\frac{x+8}{(x-3)(x-4)(x-5)}=\frac{x-3+11}{(x-3)(x-4)(x-5)}&=\frac{x-3}{(x-3)(x-4)(x-5)}+\frac{11}{(x-3)(x-4)(x-5)}\\&=\frac{1}{(x-4)(x-5)}+\frac{11}{(x-3)(x-4)(x-5)}\\&=(x-6)^{(-2)}+11(x-6)^{(-3)}\end{align*}$

## Shifting Operator 
**First Shifting operator**

$$\begin{align*}Ef(x)&=f(x+h)\\E^2f(x)&=f(x+2h)\\E^3f(x)&=f(x+3h)  \end{align*}$$


The general power of E is defined by the equation $E^nf(x)=f(x+nh)$

## Divided Difference 
- Properties 
- Any divided difference of the sum (or difference) of two functions is equal to the sum (or difference) of the divided difference of  the individual function 
- Any divided difference of a constant times a function is equal to the constant times the difference of the function.
- Note: A divided difference of any order is defined as the difference between two divided differences of the next lower order, overlapping in all but one of their arguments, divided by the difference between the extreme or non -overlapping arguments appearing in these differences. 
- If $f(x_i)$ and $f(x_i)$ are any two values of $f(x)$, then the first divided difference of $f(x)$ are defined by the formula
- $f(x_i,x_j)=\frac{f(x_i)-f(x_j)}{x_i-x_j}$
- **The Second Divided Difference** 
	- Similarly, if $f(x_i,x_j)$ and $f(x_j,x_k)$ are two first divided difference of $f(x)$ having one argument in common, then the second divided difference are defined by the formula 
	- $f(x_i,x_j,x_k)=\frac{f(x_i,x_j)-f(x_j,x_k)}{x_i-x_k}$
- **The Third Divided Difference**
	- The third divided difference is defined by the formula 
	- $f(x_i,x_j,x_k,x_i)=\frac{f(x_i,x_j,x_k)-f(x_j,x_k,x_l)}{x_i-x_l}$


https://youtu.be/C4JjFL65p0I?si=gWCm3Q0Nnf0sClDg

## Forward or advancing difference 
**The First Forward or Advancing Difference**
- The first forward or advancing difference is defined by $\Delta f(x)=f(x+h)-f(x)$, where h is the interval. 
- If h=1 and x=n, n is any real number $\Delta f(x)=f(x+1)-f(x)=f_{n+1}-f_n$
- The first forward difference in terms of the shifting operator E, $\Delta f(x)=Ef(x)-f(x)=(E-1)f(x)$
**The Second Forward or Advancing Difference**
- The second forward or advancing difference is defined by $\Delta ^2 f(x)=f(x+2h)-2f(x+h)+f(x)$
**The Third Forward or advancing Difference**
- The third forward or advancing difference is defined by $\Delta ^3 f(x)=f(x+3h)-3f(x+2h)+3f(x+h)-f(x)$

#### Nth Forward Difference 
- The nth Forward or Advancing Difference 
- The nth forward or advancing difference is defined by the formula $\Delta ^nf(X)=\Delta [\Delta^{n-1}f(x)]$ or $\Delta ^n f(x)=(E-1)^nf(x)$ using the binomial expansion $\Delta ^n f(x)=(E-1)^nf(x)$ using the binomial expansion $\Delta^n f(x) = [ E^n-\binom{n}{1}E^{n-1}+\binom{n}{2}E^{n-2}+...+(-1)^{n-1}\binom{n}{n-1}E+(1)^n\binom{n}{n}]$

- **Properties of Forward or Advancing Difference** 
1. $\Delta[f(x)\pm g(x)]=\Delta f(x) \pm \Delta g(x)$
2. $\Delta cf(x)=c\Delta (x)$
3. $\Delta f(x)g(x)=g(x) \Delta f(x)+f(x+h) \Delta g(x)$
4. $\Delta \frac{f(x)}{g(x)} = \frac{g(x)\Delta f(x)-f(x)\Delta g(x)}{g(x)g(x+h)}$
5. $\Delta c^x = c^x(c^h-1)$
6. $\Delta x^{(m)} = mx^{(m-1)}$


https://youtu.be/TIWRyzzFUYQ?si=egQpoLLv8IeX3Aa-


## Backward or Regressing Difference
**The First Backgward or Regressing Difference
- The  first backward or regressing difference is defined by $\nabla f(x)=f(x)-f(x-h)$
- If h=1 and x=n, n is any real number
- $\nabla f(x)=f(x)-f(x-1)=f_n-f_{n-1}$
- The first backward difference in terms of the shifting operator E, $\nabla f(x) =f(x)-E^{-1}f(x)=(1-E^{-1})f(x)$
**The Second Backward or Regressing Difference**
- The second backward or regressing difference is defined by $\nabla^2 f(x)=f(x)-2f(x-h)+f(x-2h)$
**The Third Backward or Regressing Difference**
- The third backward or regressing difference is defined by $\nabla^3f(x)=f(x)-3f(x-h)+3f(x-2h)-f(x-3h)$

#### Nth Backward Difference 
- The nth backward or Regressing Difference 
	- The nth backward or regressing difference is defined by 
- $\nabla^n f(x)=\nabla[\nabla^{n-1}f(x)]$ or $\nabla ^nf(x)=(1-E^{-1})^nf(x)$ using the binomial expansion $\nabla^n f(x)=(1-E^{-1})^nf(x)$
- $\nabla^n f(x) =[1-\binom{n}{1}E^{-1}+\binom{n}{2}E^{-2}+...(-1)^{n-1}\binom{n}{n-1}E^{-(n-1)}+E^{-n}\binom{n}{n}]f(x)$
**Properties of Forward or Advancing Difference** 
1. $\nabla[f(x)\pm g(x)] =\nabla f(x)\pm \nabla g(x)$
2. $\nabla cf(x)=c\nabla(x)$
3. $\nabla f(x)g(x)=g(x)\nabla f(x)+f(x-h)\nabla g(x)$
4. $\nabla \frac{f(x)}{g(x)}=\frac{g(x)\nabla f(x)-f(x)\nabla g(x)}{g(x)g(x-h)}$
5. $\nabla c^x=c^x(1-c^{-h})$
6. $\nabla x^{(m)}=m(x-1)^{(m-1)}$

## Central Difference
**First Central Difference**
- The first central difference is defined by $\delta f(x)=f(x+\frac{h}{2})$ or $\delta f(x)=E^{1/2}f(x)-E^{-1/2}f(x)$
**Second Central Difference**
- The second central difference is defined by $\delta ^2 f(x)=f(x+h)-2f(x)+f(x-h)$
**The third central Difference**
- The third central difference is defined by $\delta^3f(x)=f(x+\frac{3h}{2})-3f(x+\frac{h}{2})+3f(x-\frac{h}{2})-f(x-\frac{3h}{2})$

#### nth central difference 
- The nth central difference is defined by $\delta^nf(x)=\delta[\delta^{n-1}f(x)]$ or $\delta^nf(x)=(E^{1/2}-E^{-1/2})^nf(x)$ using the binomial expansions $\delta^nf(x)=(E^{1/2}-E{-1/2})^nf(x)$
- $\delta^nf(x)=[E^{n/2}-\binom{n}{1}E^{n/2-1} + \binom{n}{2}E^{n/2-2}+...+(-1)^{n-1}\binom{n}{n-1}E^{-\frac{n}{2}+1}+E^{-n/2}\binom{n}{n}]f(x)$

**Properties of Central difference**
- $\delta[f(x)\pm g(x)]=\delta f(x) \pm \delta g(x)$
- $\delta cf(x)=c\delta(x)$
- $\delta f(x)g(x)=\mu g(x)\delta f(x) + f(x) \delta g(x)$
- $\delta \frac{f(x)}{g(x)} = \frac{\mu g(x)\delta f(x) -\mu f(x) \delta g(x)}{g(x-\frac{h}{2})g(x+\frac{h}{2})}$

## Anti-Difference 
- Consider the difference of F(x)
- $\Delta F(x)=f(x)$
- $F(x)=\frac{f(x)}{\Delta}$
- The anti-difference of f(x) is defined by 
- $F(x)=\Delta ^{-1}f(x)$

## Theorem 
- If $F(i)$ is any anti-difference of $F(i)$, then the sum from $i=1$ to $i=n$ of the series whose general form is $f(i) \; is \; F(n+1)-F(1)$.

https://youtu.be/to82dv2SX28?si=ULrZUPvU5sjUwTpd



# Long Test  2 answers


1. 

| x | 0 | 1| 3 | 4| 6| 7|
|---|---|---|--|---|---|---|
|f(x) | 0|-3|15|48|192|315|
Find f(1,3,4)
$$\begin{align*} f(1,3) &= \frac{f(1)-f(3)}{1-3} &= \frac{-3-15}{-2} &= 9 \\ f(3,4) &= \frac{f(3)-f(4)}{3-4} &=\frac{15-48}{-1}&=33\\ f(1,3,4) &= \frac{f(1,3)-f(3,4)}{1-4} &= \frac{9-33}{-3}&=8\end{align*}$$

2. 

|x|0|1|2|3|4|5|
|-|-|-|-|-|-|-|
|f(x)|.5|0|5.5|23.0|58.5|118|
Find $\Delta f(3)$

$$\begin{align*}f(x+h)&-f(x)\\ f(3+1) &- f(3) \\ 58.5&-23 = 35.5\end{align*}$$

3. 
   
|x|2|4|6|8|10|
|--|--|-|-|-|-|
|f(x)|4|36|148|388|804|

Find $\nabla f(6), let x_{0}=10$

$$\nabla f(6)=f(6)-f(4)=148-367=112$$

4. 

|x|0|1|2|3|4|5|
|-|-|-|-|-|-|-|
|f(x)|4|3|4|31|132|379|

Find $\delta^{3} f\left(x_{-\frac{1}{2}}\right) if x_0=2$

|x|f(x)|$\delta f(x)$|$\delta^2f(x)$|$\delta^2f(x)$|
|-|-|-|-|-|
|0|4||||
|||-1|||
|1|3||2||
|||1||24|
|2|4||26||
|||27||48|
|3|31||74||
|||101||72|
|4|132||146||
|||247|||
|5|379||||

5. 
   Convert $(x+3)(x+4)(x+5)(x+8)$

$$\begin{align*}(x+3)(x+4)&(x+5)(x+8)\\(x+3)(x+4)&(x+5)(x+6+2)\\(x+3)(x+4)(x+5)(x+6) &+2(x+3)(x+4)(x+5)\\(x+6)^{(4)}&+2(x+5)^{(3)}\end{align*}$$

6. $(2x+1)(2x+3)(2x+5)$
   $$\begin{align*}(2x+1)(2x+3)(2x+5)\\2x^3(x+\frac{1}{2})(x+\frac{3}{2})(x+\frac{5}{2})\\8(x+\frac{5}{2})^{(3)}\end{align*}$$
7. $\frac{1}{(3x-1)(3x-4)}$ convert to factorial polynomial 
$$\begin{align*}\frac{1}{(3x-1)(3x-4)} &= \frac{1}{3^{2}(x-\frac{1}{3})(x-\frac{4}{3})} \\ \frac{1}{9(x-(\frac{4}{3}-1))} &=\frac{1}{9(x-\frac{7}{3})^{(2)}} \\ &\frac{(x-\frac{7}{3})^{(-2)}}{9}\end{align*}$$
8. $\frac{1}{(x-9)(x-10)(x-11)}$
$$\begin{align*}\frac{1}{(x-9)(x-10)(x-11)} \\ \frac{x-9+9}{(x-9)(x-10)(x-11)} &+\frac{9}{(x-9)(x-10)(x-11)}\\\frac{1}{(x-9)^{(2)}}&+\frac{9}{(x-8)^{(3)}}\\(x-9)^{(2)}&+9(x-8)^{(-3)}\end{align*}$$


9. $\Delta^{3}(x^{4}-2x^{2}+4)$

|1| |1|0|-2|0|4|
|-|-|-|-|-|-|-|
||||1|1|-1||
|2||1|1|-1|-1|
||||2|6|||
|||1|3|5||
|3|||3||||
|||1|6
|||1||||

$$\Delta^{3}(x^{(4)}+6x^{(3)}+5x^{(2)}-x+4)$$
$$\begin{align*}&=4*3*2(x-3)^{(1)}+6*3*2*1+0+0+0\\&=24x-72+36\\&=24x-36\\&=12(2x-3)\end{align*}$$




10. $\delta^{3} (4^{2x+1})$
$$\begin{align*}&\delta^{3} (4^{2x+1})\\&f(x+\frac{3h}{2})-3f(x+\frac{h}{2})+3f(x-\frac{h}{2})-f(x-\frac{3h}{2})\\ &=(4^{2(x+\frac{3}{2})}-3(4^{2(x+\frac{1}{2} )})+3(4^{2(x-\frac{1}{2})}) - 4^{2(x-\frac{3}{2})})4^{1}\\&=4(4^{(2x+3)}-3(4^{2x+1})+3(4^{(2x-1)})-4^{2x-3})\\ &= 4^{1}(4^{2x}))(4^{3}-3(4)+3(4^{-1})-4^{-3})\\ &= 4^{2x+1}(\frac{3375}{64}) \end{align*}$$

---

# FINALS
## Interpolation 

### Interpolation polynomial 

#### Examples 
$$f(2.5)=3.117 \;and\; f(2.6)=4.056. \; Find \; f(2.54)$$
$$p(x)=y_0+\frac{y_1-y_0}{x_1-x_0}*(x-x_0)$$
$$f(2.54)=f(2.5)+\frac{f(2.6)-f(2.5)}{2.6-2.5}(2.54-2.5)$$
$$f(2.54)=3.117+\frac{4.056-3.117}{0.1}(0.4)=3.493$$

### Linear Interpolation 
- Interpolation means the determination of $f(x)$ for a value of x between two tabular values 
- From analytic geometry, we defined that two distincty points $P_0(x_0,y_0)$ and $P_1(x_1,y_1)$ determined a straight line. The equation of the line can be written as 

$$p(x)=\frac{x-x_1}{x_0-x_{1}}*y_0\frac{x-x_{1}}{x_{0}-x_{1}}*y_{1}$$
It is easily verified that $p(x_{0})=y_0$ and $p(x_1)=y_1$. The polynomial p(x) whose degree n is equal to one, and is used for **linear interpolation**. 


$$p(x)=y_0+\frac{y_{1}-y_0}{x_{1}-x_0}*(x-x_0)$$

### Taylor's Polynomial 
- For greater accuracy it is necessary to use higher degree interpolation formulas 
- Polynomial interpolation provides mathematical tools that can be used in developing methods of approximation theory, numerical differentiation and numerical integration and numerical solutions of ordinary differential equations 
- The Taylor's polynomial is a truncated Taylor's series expansion 
$$f(x)=f(x_0)+f'(x_0)(x-x_0)+f''(x_0)\frac{(x-x_0)^2}{2!}+f'''(x_0)\frac{(x-x_0)^3}{3!}+...+f^{(n)}(x_0)\frac{(x-x_0)^n}{n!}+R_{n+1}(x)$$
- with the remainder term 

$$R_{n+1}(x)= \frac{1}{n!}\int^x_{c}(x-s)^{n}f^{(n+1)}(s)ds$$

### Examples 
1. Find the Taylor polynomial of degree three for $f(x)=e^{2x} \; sin \;x$ expanded about  $x_0$. 
2. Use the polynommial in (a) to approximate the function $f(0.1)$, measure the absolute error at $\epsilon = 10^{-8}$ 
3. Use the polynomial in (a) to approximate the function $f(0.01)$, measure the approximate error at $\epsilon = 10^{-8}$

$$f(x)=e^{2x}sin \; x$$
$$\begin{align*}f'(x)&=2e^{2x}sinx+e^{2x}cosx\\f''(x)&=4e^{2x}sinx+2e^{2x}cosx+2e^{2x}cosx-e^{2x}sinx\\&=3e^{2x}sinx +4e^{2x}cosx\\f'''(x)&=6e^{2x}sinx+3e^{2x}cosx+8e^{2x}cosx-4e^{2x}sinx\\&=2e^{2x}sinx+11e^{2x}cosx\end{align*}$$
$$\begin{align*}f(0)&=0\\f'(0)&=1\\f''(0)&=4\\f'''(0)&=11\end{align*}$$

$$P_3(x)=0+x+\frac{4}{2!}x^2+\frac{11}{3!}x^3=x+\frac{4}{2!}x^2+\frac{11}{6}x^3$$
$$P_3(x)=x+2x^2+\frac{11}{6}x^3$$
Now taking x = 0.1, we get the estimate value $P_3(0.1)=0.12183333$ 
The actual value is 

$$f(0.1)=e^{2(0.1)}sin(0.1)=0.12193681$$




### Interpolation by the Shifting operator 
- Interpolation using the shifting operator 
- Given a sequence $S_1,S_2,...,S_k,...,S_n$
- Use $(E-1)^{n-1}f(x)=0$

#### Example 

|x|2.1|2.2|2.3|2.4|2.5|
|-|-|-|-|-|-|
|f(x)|5.671|6.832|7.115|?|8.934|

h=0.1

$$\begin{align*}E^nf(x)&=f(x+nh)\\(E-1)^4&f(2.1)=0\\(E^4-4&E^3+6E^{2}-4E+1)f(2.1)=0\\f(2.5)-4f&(2.4)+6f(2.3)-4f(2.2)+f(2.1)=0\\f(2.5)+&6f(2.3)-4f(2.2)+f(2.1)=4f(2.4)\end{align*}$$
$$f(2.4)=\frac{f(2.5)+6f(2.3)-4f(2.2)+f(2.1)}{4}$$
$$f(2.4)=\frac{8.934+6(7.115)-4(6.832)+5.671}{4}=7.492$$



### Polynomial Interpolation 
- Polynomial interpolation provides mathematical tools that can be used in developing methods of approximation theory, numerical differentiation and numerical integration and numerical solutions of ordinary differential equations. 
- **Taylor's Polynomial**
	- The Taylor's polynomial is a truncated Taylor's series expansion

$$f(x)=f(x_0)+f'(x_0)(x-x_0)+f''(x_0)\frac{(x-x_0)^2}{2!}+f'''(x_0)\frac{(x-x_0)^3}{3!}+...+f^{(n)}(x_0)\frac{(x-x_0)^n}{n!}+R_{n+1}(x)$$

#### Example 

a. Find the Taylor polynomial degree three for $f(x) = e^{2x} sin \; x$ expanded about $x_0=0$. b. Use the polynomial in (a) to approximate the function $f(0.1)$ 

Solution. The third degree Taylor polynomial expanded about $x_0$ is 

$$f(x)= f(x_{0)}+ f'(x_0)(x-x_0)+f''(x_0)\frac{(x-x_0)^2}{2!}+f'''(x_0)\frac{(x-x_0)^3}{3!}$$

with the remainder 

$$R_4(x)=f^{(IV)}(x_0)\frac{(x-x_0)^4}{4!}$$
Calculating the derivatives 

$$\begin{align*}f(x)&=e^{2x}sinx\\f'(x)&=2e3^{2x}sinx+e^{2x}cosx\\f''(x)&=3e^{2x}sinx+4e^{2x}cosx\\f'''(x)&=2e^{2x}sinx+11e^2xcosx\end{align*}$$
Setting $x_0=0$

$$\begin{align*}f(0)&=0\\f'(0)&=1\\f''(0)&=4\\f'''(0)&=11\end{align*}$$

Putting all this values gives 

$$P_3(x)=x+2x^2+\frac{11}{6}x^3$$
Now taking x=0.1, we estimate value $P_3(0.1)=0.121833333$
The actual value 

$$f(0.10)=e^{2(0.1)} sin(0.1)=0.12193681$$


### Interpolation for Unequal Intervals
When the data points in a given sequance function are not equally spaced 

|$x$|$x_0$|$x_1$|...|$x_n$|
|-|-|-|-|-|
|$f(x)$|$f(x_0)$|$f(x_1)$|...|$f(x_n)$|

that is 
$x_1-x_0 \neq x_{2}-x_{1}\neq...\neq x_{n}-x_{n-1}$


### Lagrange Interpolation Formula 
- The Lagrange interpolation method provide a direct approach for determining  
interpolated values regardless of data points spacing, that is, it can be fitted to unequally spaced  
or equally spaced data.

Suppose the values of a function $p(x)$ is known at n + 1 nodes $x_0,x_1,...,x_n$ say, given two pints $(x_0,f(x_{0))} \; and \; (x_1,f(x_1))$ 

$$p_{1(x)}= \frac{x-x_1}{x_0-x_{1}}f(x_{0)}+ \frac{x-x_0}{x_1-x_0}f(x_1)$$
For three points, $(x_0,f(x_0)),(x_1,f(x_1)),...,(x_2,f(x_2))$

$$p_2(x)=\frac{(x-x_1)(x-x_2)}{(x_0-x_1)(x_0-x_2)}f(x_0)+\frac{(x-x_0)(x-x_2)}{(x_1-x_0)(x_1-x_2)}f(x_1)+\frac{(x-x_0)(x-x_1)}{(x_2-x_0)(x_2-x_1)}$$

For n points, $(x_0,f(x_0)),(x_1,f(x_1)),...,(x_n,f(x_n))$

$$p_n(x)=\frac{(x-x_1)(x-x_2)...(x-x_n)}{(x_0-x_1)(x_0-x_2)...(x_0-x_n)}f(x_0)+\frac{(x-x_0)(x-x_2)...(x-x_n)}{(x_1-x_0)(x_1-x_2)...(x_1-x_n)}f(x_1)+...+\frac{(x-x_0)(x-x_1)...(x-x_{n-1})}{(x_n-x_0)(x_n-x_1)...(x_n-x_{n-1})}f(x_n)$$

#### Examples 
1. Consider the following table: 

|x| 0|2|5|
|-|-|-|-|
|f(x)|-1|9|39|
a. Construct the interpolation polynomial to approximate the function using the suitable Lagrange interpolation formula
b. Use the polynomial in (a) to interpolate $f(x)$ at x=10 

Solution 
A quadratic polynomial can be determined so that is passes through the three points 

$$p_2(x)=L_0(x)f(x_0)+L_1(x)f(x_1)+L_2(x)f(x_2)$$
<center>or</center>
$$p_2(x)=(-1)L_0(x)+9L_1(x)+39L_2(x)$$
The Lagrange coefficients can be calculated: 


$$L_0(x)=\frac{(x-x_1)(x-x_2)}{(x_0-x_1)(x_0-x_2)}=\frac{(x-2)(x-5)}{(0-2)(0-5)}=\frac{1}{10}(x^2-7x+10)$$
$$L_{1}(x)=\frac{(x-x_0)(x-x_2)}{(x_1-x_0)(x_1-x_{2})}=\frac{(x-0)(x-5)}{(2-0)(2-5)}=-\frac{1}{6}(x^2-5x)$$
$$L_2(x)=\frac{(x-x_0)(x-x_1)}{(x_2-x_0)(x_2-x_1)}=\frac{(x-0)(x-2)}{(5-0)(5-2)}=\frac{1}{15}(x^2-2x)$$

Putting these values together 

$$p_2(x)=-\frac{1}{10}(x^2-7x+10)-\frac{3}{2}(x^2-5x)+\frac{39}{15}(x^2-2x)$$
$$=x^2+3x-1$$
$$p_2(10)=12$$

2. Find the interpolating polynomial of degree less than or equal to 3 of the points (-1,3), (0,2), (2,0) and (4,-1). 

Evaluate p(1)


Solution. Using Lagrange Formula 

$$\begin{align*}p(x)&=\frac{(x)(x-2)(x-4)}{(-1)(-1-2)(-1-4)}*3 +\frac{(x+1)(x-2)(x-4)}{(0+1)(0-2)(0-4)}*(2)+\frac{(x+1)(x)(x-4)}{(2+1)(2)(2-4)}*0+\frac{(x+1)(x)(x-2)}{(4+1)(4)(4-2)}*(-1)\\p(x)&=-\frac{1}{5}(x^3-6x^2+8x)+\frac{1}{4}(x^3-5x^2+2x+8)+0(x^3-x^2-2x)\\p(x)&=\frac{1}{40}x^3-\frac{1}{40}x^2-\frac{21}{20}x+2\end{align*}$$
Now

$$p(1)=\frac{1}{40}(1)^3-\frac{1}{40}(1)^2-\frac{21}{20}(1)+2$$
$$p(1)=\frac{12}{20}$$

### Interpolation for Unequal Intervals 

- When the data points in a given sequence function are not equally spaced, 

|$x$|$x_{0}$|$x_1$|$...$|$x_n$|
|-|-|-|-|-|
|$f(x)$|$f(x_0)$|$f(x_1)$|$...$|$f(x_n)$|

that is, 

$$x_1-x_{0}\neq x_{2}- x_{1}\neq ...\neq x_{n}-x_{n-1}$$
#### Lagrange formula
- Let 

$$L_0(x)=\frac{(x-x_{1})(x-x_2)...(x-x_n)}{(x_0-x_1)(x_0-x_2)...(x_0-x_n)}$$
$$L_1(x)=\frac{(x-x_0)(x-x_2)...(x-x_n)}{(x_1-x_0)(x_1-x_2)...(x_1-x_n)}$$
$$....$$
$$L_n(x)=\frac{(x-x_0)(x-x_1)...(x-x_{n-1})}{(x_n-x_0)(x_n-x_1)...(x_n-x_{n-1})}$$

<center>
Rewriting the formula
</center>

$$p(x)=L_0(x)f(x_0)+L_1(x)f(x_1)+...+L_n(x)f(x_n)$$


### Theorem. (Existence and Uniqueness of Polynomial Interpolation)

**Theorem (Existence and Uniqueness of Polynomial Interpolation)**. If points $x_0,x_1,...,x_n$ are distinct, then for any arbitrary real values $y_0,y_1,...,y_n$, there is a unique polynomial $p(x)$ of degree at most n such that $p(x_i)=y_i$ for $0\leq i \leq n$. 

**Proof**. The Lagrange Polynomial construction gives exstence of such a polynomial $p(x)$ of degree at most n.

Suppose there exists two polynomials $p(x)$ and $q(x)$ whose degree are both at most n are both interpolating the data. Let $r(x)=p(x)-q(x)$ which can have a degree of at most $n$ also, it has roots at $x_0,x_1,...,x_n$. The only polynomial of degree at most n has n+1 distinct roots is the zero polynomial. Therefore, it only implies that p(x) and q(x) are equal everywhere. 
### The Newton's Divided Difference interpolation formula 
- Given the points $(x_{0,}f(x_{0)),}(x_1,f(x_1)),...,(x_n,f(x_n))$
- Construct the divided difference table 
- Solve for the divided differences $f(x_0,x_1),f(x_0,x_1,x_2),f(x_0,x_1,x_2,x_3),...$

$$f_x=f_0+(x-x_0)f(x_0,x_1)+(x-x_0)(x-x_1)f(x_0,x_1,x_2)+(x-x_0)(x-x_1)(x-x_2)f(x_0,x_1,x_2,x_3)+(x-x_0)(x-x_1)(x-x_2)(x-x_3)(x-x_4)+...$$

|$x$|$f(x)$|$f(x_0,x_1)$|$f(x_0,x_1,x_2)$|$f(x_0,x_1,x_2,x_3)$|$f(x_0,x_1,x_2,x_3,x_4)$|
|-|-|-|-|-|-|
|1|1|
|||31|
|5|125||6
|||25||1|
|0|0||12||0|
|||49||1|
|7|343||9||0|
|||67||1|
|2|8||15||0|
|||52||1|
|6|216||17|
|||171|
|9|729|

- The first difference is the highlighted part 

|$x$|$f(x)$|$f(x_0,x_1)$|$f(x_0,x_1,x_2)$|$f(x_0,x_1,x_2,x_3)$|$f(x_0,x_1,x_2,x_3,x_4)$|
|-|-|-|-|-|-|
|1|**1**|
|||**31**|
|5|125||**6**
|||25||**1**|
|0|0||12||**0**|
|||49||1|
|7|343||9||0|
|||67||1|
|2|8||15||0|
|||52||1|
|6|216||17|
|||171|
|9|729|

- Using hte newtons interpolatuion formula 

$$f_x=f_0+(x-x_0)f(x_0,x_1)+(x-x_0)(x-x_1)f(x_0,x_1,x_2)+(x-x_0)(x-x_1)(x-x_2)f(x_0,x_1,x_2,x_3)$$
$$x_0=1$$
$$f_x=1+(x-1)(31)+(x-1)(x-5)(6)+(x-1)(x-5)+(x-1)(x-5)(x-0)(1)$$
$$f_x=1+31x-31+6x^2-36x+30+x^3-6x_2+5x=x^3$$
$$x_0=0$$
$$f_x=0+(x-0)(49)+(x-0)(x-7)(9)+(x-0)(x-7)(9)+(x-0)(x-7)(x-2)(1)$$
$$f_x=0+49x-31+6x^2-36x+30+x^3-6x^2+5x=x^3$$




### Interpolation for Even Intervals 
- The study of interpolation to equally spaced data is important in evaluating tabulated functions. The Newton's interpolation formulas are derived from the Newton's divided difference formula 

**The Gregory-Newton Interpolation fromula**
- Suppose the numerical values of f(x) are given for values where the argument x increase by equal interval h. 
- $f_1-f_0=\Delta f_0$
- $f_1=f_{0}+\Delta f_0$
- $f_{2}-f_{1} = \Delta f_1$

$$\begin{align*}f_2&=f_{1}+ \Delta f_{1}=f_{0}+\Delta f_{0}+\Delta f_{0}+ \Delta ^{2}f_{0}\\&=f_{0}+2\Delta f_{0}+\Delta ^{2}f_{0}\\&=(1+\Delta)^2f_0\end{align*}$$

which may be written 
### Gregory-Newton Interpolation Formulas
- contiuing in this manner $f_n$ may be expressed in the form 
- $f_{n}= (1+\Delta)^nf_{n}$
- Using the binomial theorem to expand this gives the Gregory-Newton formula of interpolation 
- $f_n=f_{0}n\Delta f_{0}+\frac{n(n-1)}{2!}\Delta ^{2}f_{0}+ \frac{n(n-1)(n-2)}{3!} \Delta ^{3}f_{0}+ \frac{n(n-1)(n-2)(n-3)}{4!}\Delta ^{4}f_{0}+ ...$
or 

$f_{n}= f_{0}+(n)^{(1)} \Delta f_{0}+\frac{(n)^{(2)}}{2!}\Delta ^{2}f_0+\frac{(n)^{(3)}}{3!}\Delta ^{3}f_{0}+ \frac{(n)^{(4)}}{4!}\Delta ^{4}f_{0}+...$

### Gregory-Newton Forward Difference Interpolation Formulas
- Here n is a positive integer but the result still hods for fractional and negative values. Thus if we require $f_{r}$ where r is a fraction of the interval h we have 

$f_r=f_{0}+r \Delta f_{0}+ \frac{r(r-1)}{2!}\Delta ^{2}f_{0}+\frac{r(r-1)(r-2)}{3!}\Delta ^{3}f_{0}+ \frac{r(r-1)(r-2)(r-3)}{4!} \Delta ^{4}f_{0}+ ...$

or 

$f_{r}= f_{0}+r^{(1)}\Delta f_{0}+ \frac{(r)^{(2)}}{2!}\Delta ^{2}f_{0}+\frac{(r)^{(3)}}{3!}\Delta ^{3}f_{0}+\frac{(r)^{(4)}}\Delta ^{4}f_0+...$

To find $P_x$

$P_{x}= f_{0}+x \Delta f_{0} + \frac{x(x-1)}{2!} \Delta ^{2} f_{0} + \frac{x(x-1)(x-2)}{3!} \Delta ^{3}f_{0} + \frac{x(x-1)(x-2)(x-3)}{4!}\Delta ^{4} f_{0}+ ...$

or

$P_{x}= f_{0}+x(x)^{(1)}\Delta f_{0}+ \frac{(x)^{(2)}}{2!} \Delta ^{2}f_{0} + \frac{(x)^{(3)}} \Delta ^{3}f_{0}+\frac{(x)^{(4)}}{4!} \Delta ^{4}f_{0}+...$

To find $P_{x}$ if $h \neq 1$

$P_{x}=f_{0}+ \frac{(x-x_0)}{1!h}\Delta f_{0}+\frac{(x-x_0)(x-x_1)}{2!h^{2}}\Delta ^{2} f_{0}+\frac{(x-x_{0})(x-x_{1})(x-x_{2})}{3!h^{3}}\Delta ^{3}f_{0}+ \frac{(x-x_0)(x-x_1)(x-x_2)(x-x_3)}{4!h^{4}}\Delta^4f_0+....$


### Newton Backward Difference Interpolation Formula 

$$P_{x}= f_{0}+ \frac{(x-x_{0})}{1!h_{0}}\nabla f_{0}+ \frac{(x-x_0)(x-x_{1)}}{2!h^{2}}\nabla^{2}f_{0}+\frac{(x-x_0)(x-x_1)(x-x_2)}{3!h^3}\nabla^{3}f_{0+}\frac{(x-x_0)(x-x_1)(x-x_2)(x-x_3)}{4!h^{4}} \nabla^{4}f_0+...$$


$$f_r=f_{0}+r\nabla f_{0}+\frac{r(r+1)}{2!}\nabla ^{2}f_{0}+\frac{r(r+1)(r+2)}{3!}\nabla^3f_{0}+\frac{r(r+1)(r+2)(r+3)}{4!}\nabla^4f_0+...$$

1. For the following values of $f(x)$ from x = 0 to x = 5, tabulate the finite difference of $f(x)$ to the fourth order. 

	Find 
		a. $f(10)$
		b. $f(\frac{1}{2})$
		c. $f(x)$

|x|0|1|2|3|4|5|
|-|-|-|-|-|-|-|
|f(x)|-3|-6|-11|-12|-3|22

Solution 

|$x$ | $f(x)$|$\Delta f(x)$ | $\Delta ^{2}f(x)$| $\Delta ^{3}f(x)$ | $\Delta ^{4}f(x)$|
|-|-|-|-|-|-|
|0|-3|
|||-3|
|1|-6||-2|
|||5||6||
|2|-11||4||0|
|||-1||6
|3|-12||10||0
|||9||6
|4|-3||16
|||25|
|5|22|

$$f_{n}= f_{0}+n\Delta f_{0}+ \frac{n(n-1)}{2!}\Delta ^{2}f_{0}+ \frac{n(n-1)(n-2)}{3!}\Delta ^{3}f_{0}+\frac{n(n-1)(n-2)(n-3)}{4!}\Delta ^4f_{0}+...$$
$$x_{0}= 0$$

$$f_{10}=(-3)+(10)(-3)+ \frac{(10)(9)}{2!}(-2)+\frac{(10)(9)(8)}{3!}(6)=597$$

$$f_{1/2}=(-3)+(\frac{1}{2})(-3)+\frac{(\frac{1}{2})(-\frac{1}{2})}{2!}(-2)+\frac{x(x-1)(x-2)}{3!}(6)=x^{3}-4x^{2}-3$$

$$x_0=2$$

$$f_{x}=(-11)+(x-2)(-3)+\frac{(x-2)(x-3)}{2!}(-2)+\frac{(x-2)(x-3)(x-4)}{3!}(6)$$

|$x$|$f(x)$|$\Delta f(x)$|$\Delta ^2f(x)$|$\Delta ^3f(x)$|$\Delta ^4f(x)$|
|-|-|-|-|-|-|
|0.50|0.875|
|||-0.625|
|1.00|0.250||0.500|
|||-0.125||0.750|
|1.50|0.125||1.250||0|
|||1.125||0.750|
|2.00|1.250||2.000||0|
|||3.125||0.750|
|2.50|4.375||2.750|
|3.00|10.250||

$$f_{r}=f_{0}+r^{(1)}\Delta f_{0}+\frac{(r)^{(2)}}{2!} \Delta ^{2}f_{0}+ \frac{(r)^{(3)}}{3!}\Delta ^{3}f_{0}+ \frac{(r)^{(4)}}{4!}\Delta ^{4}f_{0}+....$$

Find $f(1.25)$ if $x_{0}=1.00$

$$1.25 = 1.00 r(0.50)$$
$$r=\frac{1.25-1.00}{0.5} = 0.5$$

$$f_{1.25}=0.250+(0.5)^{(1)}(-0.125)+\frac{(0.5)^{(2)}}{2!}(1.250)+ \frac{(0.5)^{(3)}}{3!}(0.750)$$

Find $f(2.75)$ if $x_{0}=2.00$

$$2.75 = 2.00 + r(0.50)$$
$$r=\frac{2.75-2.00}{0.5}=1.5$$

$$f_{2.75}= 1.250+(1.5)^{(1)}(3.125)+\frac{(1.5)^{(2)}}{2!}(2.750)+\frac{(1.5)^{(3)}}{3!}(0.750)$$

$$P_x=f_{0}+\frac{(x-x_0)}{1!h}\Delta f_{0}+\frac{(x-x_{0})(x-x_{1})}{2!h^{2}\Delta}^{2}f_{0}+\frac{(x-x_0)(x-x_{1})(x-x_2)}{3!h^{3}\Delta}^{3}f_{0} + \frac{(x-x_0)(x-x_2)(x-x_3)}{4!h^{4}} \Delta ^{4}f_0+.....$$

$$P_{x}= 1.250 + \frac{(x-2)}{1!(0.5)}(2.125)+\frac{(x-2)(x-2.5)}{2!(0.5)^2}(2.750)+\frac{(x-2.0)(x-2.5)(x-3.0)}{3!(0.5)^3}(0.750)$$


### The Gauss Central Difference Interpolation Formulas

#### The Gauss Forward Central Difference Formula 

$$f_{x}= f_{x_{0}}+\frac{x-x_0}{h}\delta f_{1/2}+\frac{(x-x_{0})(x-x_{1})}{2!h^{2}}\delta^2f_0+\frac{(x-x_{-1})}{3!h^{3}}\delta ^{3} f_{1/2}+\frac{(x-x_{-1})(x-x_0)(x-x_1)(x-x_2)}{4!h^4}\delta^4f_0+...$$

$$\text{or}$$
$$f_{x}=f(x_{0}+rh)= f_{0}+r\delta f_{1/2}+\frac{(r)(r-1)}{2!}\delta^0 f_0 + \frac{(r+1)(r)(r-1)}{3!}\delta^3f_{1/2}+\frac{(r+1)(r)(r-1)(r-2)}{4!}\delta^4f_0+.....$$

#### The Gauss Backward Central Difference Formula 
$$f_x=f_{x_0}+\frac{x-x_0}{h}\delta f_{-1/2}+\frac{(x-x_1)(x-x_0)}{2!h^2}\delta^2f_0+\frac{(x-x_1)(x-x_0)(x-x_1)}{3!h^3}\delta ^3 f_{1/2}+\frac{(x-x_{-2})(x-x_{-1})(x-x_0)(x-x_1)}{4!h^4}\delta^4 f_0+ ...$$

or 


$$f_x=f(x_0+rh) = f_0+r\delta f_{-1/2}+\frac{(r+1)(r)}{2!}\delta^2f_0+ \frac{(r+1)(r)(r-1)}{3!}\delta^3f_{-1/2}+\frac{r(r+1)(r+2)(r+3)}{4!}\Delta ^4f_0+.....$$