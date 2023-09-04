
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

### Mean value theorem for Derivatives 
- If f(x) is continous on the (closed and finite) interbal [a,b] and differentiable on (a,b) then 

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
![[Pasted image 20230817145440.png]]
$$\begin{align*} &\text{If } a_1 \geq a_2 \geq ... \geq a_n...0 \text{for all n in } \lim_{n \to n} a_n = 0,\\ &\text{then the alternating series} \end{align*}$$
$$a_1 - a_2 + a_3 - a_4 + ...$$
$$\text{converges, that is}$$
$$\lim_{n \to \infty} \sum\limits_{k=1}^n (-1)^{k-1}????$$

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

TrueError = TrueValue - ApproximateValue 

The relative true error which is the ratio between the true error and the true value, i.e,

$$RelativeError = \frac{TrueError}{TrueValue}$$
#### Example

$$\begin{align*}f(x)=\sqrt{x}=x^{\frac{1}{2}}  \;\;,x=5 \end{align*}$$
$$f'(x)=\frac {1}{2}x^{-\frac{1}{2}} = \frac{1}{2\sqrt{x}}$$
$$f'(x) = \frac {1}{2\sqrt{5}}=$$
$$f'(x)= \lim_{h \to 0}\frac{f(x+h)-f(x)}{h}$$
$$f'(x)\approx \frac{f(x+h)-f(x)}{h}, \;\; h=0.1, \;\; x=5$$

$$\text{The true value is}$$
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
No available notes 


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
2. Choose a convergence parameter $ \epsilon > 0 $
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
- where $\epsilon(x)$ lies between $\bar{x}$ and $x$. Since $f(p)=0$, this equation with $x=p$ gives 
$$0=f(\bar{x})+(p-\bar{x})f'(x)+\frac{(p-\bar{x})^2}{2!}f''(\epsilon(p))$$
- Newton's method is derived by assuming that, since $|\bar{x}-p|$ is small. the term involving $(p-\bar{x})^2$ is negligible and that 
$$0 \approx \bar{x} - \frac{f(\bar{x})}{f'(x)}$$
- This set the stage for the Newton-Raphson method, which starts with an initial approximation $p_0$ and generates the sequence {$p_n$} defined by 
$$p_n = p_{n-1} - \frac{f(p_n-1)}{f'(p_n-1)}$$


Starting with the initial approximation the approximation $p_0$, the approximation $p_1$ is the x-intercept of the tangent lint to the graph of f at $(p_0, f(p_0))$. The approximation $p_2$ is the x-intercept fo the tangent line to the graph of f at $(p_1, f(p_1))$, and so on.

Example 

To obtain the unique solution to $x^3+4x^2-10=0$ on the interval [1,2] by Newton's Method, generates the sequence ${p_n}^\infty_{n=0}$ by
$p_n = p_{n-1}-\frac{p^3_{n-1}+4p^2_{n-1}-10}{3p^2_{n-1}+8p_{n-1}}$

$$f(x)=x^3-4x^2-10$$
$$f'(x) = 3x^3-8x$$


$$p_1 = p_{0-1}-\frac{p^3_{0-1}+4p^2_{0-1}-10}{3p^2_{0-1}+8p_{0-1}}$$
$$p_2 = p_{1-1}-\frac{p^3_{1-1}+4p^2_{1-1}-10}{3p^2_{1-1}+8p_{1-1}}$$

#### Procedures of the Newton's Method 
1. Find the initial approximation $x_0$ for the root by sketching the graph of the function 
2. Evaluate the function $f(x)$ and the derivative $f'(x)$ at the initial approximation 
3. Check if $f(x_0)=0$ then $x_0$ is the desired approximation to a root. But if $f'(x_0)=0$, then go back to step 1 to choose a new approximation 
4. Establish the tolerance $(\epsilon>0)$ value for the function
5. Compute a new approximation for hte root using iterative formula
6. Check the tolerance. If $|f(x_n)|\leq\epsilon$, for $n\geq0$, then end; otherwise go back to step 4 and repeat the process. 

