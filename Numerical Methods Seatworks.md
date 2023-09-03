
## Seatwork #1 - 2023-08-12

Find the suitable value for c that satisfies the conclusion of Rolle's Theorem or Mean Value Theorem 

1.  $$f(x) = x^2-3x-10, [-2, 5]$$
$$ \begin{align*} f(-2)&=(-2)^2-3(-2)-10\\&=4+6-10\\&=0 \end{align*} $$
$$ \begin{align*} f(5)&=5^2-3(5)\\&=25-15-10\\&=0 \end{align*}$$
$$f(-2) \neq f(5)$$
$$ \begin{align*} &f'(x)=2x-3\\&f'(c)=2c-3 \end{align*} $$
$$\begin{align*} \frac {f(b)-f(a)}{b-a} &= 2c-3 \\ \frac {0-0}{5--2} &= 2c-3 \\ \frac {0}{7} &= 2c-3 \\ 0 &= 2c-3 \\ \frac {3}{2} &=c\end{align*}$$
2. $$f(X) = x^2-16,   [-4,4]$$
   $$\begin{align*} f(-4)&=-4^2 -16 \\ &=16-16 \\ &=0\end{align*}$$
   $$\begin{align*}f(4)&=4^2-16 \\ &=16-16 \\ &=0  \end{align*}$$
   $$\begin{align*} f'(x) =2x \\ f'(c) =2c\end{align*}$$

$$ \begin{align*} 2c&=0\\ c&=0\end{align*} $$
3. $$ f(x) = x^2 - 6x + 8, [2,4] $$
   $$ \begin{align*}f(2) &= 2^2 - 6(2) +8 \\ &=4-12+8 \\ &=0\end{align*}$$
   $$\begin{align*} f(4) &= 4^2 -6(4)+8 \\ &=16-24+8 \\ &=0 \end{align*}$$
   $$ f(2)  =  f(4) $$
   $$ \begin{align*} f'(x) = 2x-6 \\ f'(c) = 2c-6\end{align*}$$
   $$ \begin{align*} 2c - 6 &= 0 \\ c &= \frac {6}{2} \\ c &= 3\end{align*} $$
4. $$ f(x) = x^2+3x-18, [-6,3] $$
   $$\begin{align*} f(-6) &= (-6)^2 + 3(-6) - 18 \\ &=36+18-18 \\ &=0\end{align*}$$
   $$ \begin{align*}  f(3) &= 3^2 + 3(3) - 18 \\ &= 9+9-18 \\ &=0 \end{align*} $$
   $$ \begin{align*} f'(x)=2x+3 \\ f'(c)=2c+3 \end{align*} $$
   $$\begin{align*} 2c +3 &= 0 \\ c &= -\frac {3}{2}\end{align*}$$
5. $$f(x) = 4x^2 -16x+15, [\frac {3}{2}, \frac {5}{2}]$$
   $$ \begin{align*} f(\frac {3}{2}) &= 4(\frac {3}{2})^2 - 16(\frac {3}{2}) +15 \\ &=25-40+15 \\ &= 0 \end{align*} $$
   $$ \begin{align*} f(\frac {5}{2}) &= 4(\frac {5}{2})^4 - 16(\frac {5}{2}) + 15 \\ &= 25-40+5 \\ &=0\end{align*} $$
   $$\begin{align*} f'(x)=8x-16 \\ f'(c)=8-c16 \end{align*}$$
   $$  \begin{align*} 8c -16 &= 0 \\ c &= \frac {16}{8} \\ c &= 2 \end{align*} $$



## Seatwork #2 - 2023-08-17

Write the approximate polynomial of the following transcendental functions using the Maclaurin's series of approximation 
1. $$f(x) = e^{-2x}$$
   $$f(0)=1$$
   $$ \begin{align*} f'(x) &= -2 e^{-2x}, P'(0)=-2 \\ f''(x) &=4e^{-2x},P''(0)=4\end{align*} $$
$$\text{Therefore the approximate polynomial is}$$
$$\begin{align*} p(x) &= f(0)+(x-0)\frac {f'0}{1!}+(x-0)^2 \frac{f''(0)}{2!}+...\\&=1+x \frac {-2}{1!} + x^2 \frac {4}{2}+... \\ &= 1-2x+2x^2+...\end{align*}$$


2. $$ f(x)=ln(x+1) $$
   $$ \begin{align*} f(0) &= ln(1)=0 \\ f'(x) &= \frac {1}{x+1} \\ f'(0) &= 1 \\ f''(x) &= -\frac {2}{(x+1)^2}\\ f''(0) &= \frac {2}{(x+1)^3} \\ f'''(0) &= 2 \end{align*}$$
$$\text{There the approximate polynomial}$$
$$\begin{align*} p(x) &= f(0) + (x-0) \frac {f'(0)}{1!} + (x-0)^2 \frac{f''(0)}{2!} + (x-0)^3 \frac {f'''(0)}{3!} +...\\ &= 0+1*x-\frac{1}{2} * x^2 + \frac{2}{6}* x^3 + ... \\ &=x-\frac {x^2}{2} + \frac {x^3}{3} +...  \end{align*}$$


## Seatwork #3 - 2023-08-17

use the binomial theorem to expand and simplify the expression 

1. $$(x+\frac{1}{2})^5$$
<center>
<table>  
  <tr>  
    <th>1</th>  
    <th>5</th>  
    <th>10</th>  
    <th>10</th>
    <th>5</th>
    <th>1</th>
  </tr>  
</table>
</center>
$$1(x)^5(\frac {1}{2})^0 + 5(x)^4(\frac {1}{2})^1+10(x)^3(\frac {1}{2})^2+10(x)^2(\frac {1}{2})^3+5(x)^1(\frac {1}{2})^4+1(x)^0(\frac {1}{2})^5$$
$$= x^5+\frac{5x^4}{2}+\frac{10x^3}{2}+\frac{10x^2}{2}+\frac{5x}{2}+\frac{1}{32}$$

2. $$(x+1)^8$$
   <center>
<table>  
  <tr>  
    <th>1</th>  
    <th>8</th>  
    <th>28</th>  
    <th>56</th>
    <th>70</th>
    <th>56</th>
    <th>28</th>
    <th>8</th>
    <th>1</th>
  </tr>  
</table>
</center>
$$\begin{align*}&1(x)^8(1)^0+8(x)^7(1)^1+28(X)^6(1)^2+56(x)^5(1)^3+70(x)^4(1)^4+\\&56(x)^3(1)^5+70(x)^4(1)^4+56(x)^3(1)^5+28(x)^2(1)^6+8(x)^1(1)^7\\&+1(x)^0(1)^8 \end{align*}$$

$$= x^8 +8x^7+28x^6+ 56x^5+40x^4+56x^3+28x^2+8x+1 $$

3. $$(1-2y)^4$$
   <center>
<table>  
  <tr>  
    <th>1</th>  
    <th>4</th>  
    <th>6</th>  
    <th>4</th>
    <th>1</th>
  </tr>  
</table>
</center>
$$1(1)^4(-2y)^0+4(1)^3(-2y)^1+6(1)^2(-2y)^2+4(1)^1(-2y)^3+1(1)^0(-2y)^4$$
$$=1-8y-24y^2-32y^3-16y^4$$
4. $$(x-3)^6$$
<center>
<table>  
  <tr>  
    <th>1</th>  
    <th>6</th>  
    <th>15</th>  
    <th>20</th>
    <th>15</th>
    <th>6</th>
    <th>1</th>
  </tr>  
</table>
</center>
$$\begin{align*} &1(x)^6(-3)^0+6(x)^5(-3)^1+15(x)^4(-3)^2+20(x)^3(-3)^3+\\&15(x)^2(-3)^4+6(x)^1(-3)^5+1(x)^0(-3)^6\end{align*}$$

$$=x^6-18x^5+135x^4-540x^3+1215x^2-1458x+759$$
5. $$ (3x+4)^6 $$
   <center>
<table>  
  <tr>  
    <th>1</th>  
    <th>6</th>  
    <th>15</th>  
    <th>20</th>
    <th>15</th>
    <th>6</th>
    <th>1</th>
  </tr>  
</table>
</center>
$$ 1(3x)^6(4)^0+6(3x)^5(4)^1+15(3x)^4(4)^2+20(3x)^3(4)^3+15(3x)^2(4)^4+6(3x)^1(4)^5+1(3x)^0(4)^6$$
$$=729x^6+5832x^5+19440x^4+34560x^3+18432x+4096$$

6.$$(2x+3)^5$$
<center>
<table>  
  <tr>  
    <th>1</th>  
    <th>5</th>  
    <th>10</th>  
    <th>10</th>
    <th>5</th>
    <th>1</th>
  </tr>  
</table>
</center>
	$$1(2x)^5+5(2x)^4(3)^1+10(2x)^3(3)^2+10(2x)^2(3)^3+5(2x)^1(3)^4+1(2x)^0(3)^5$$
	$$=32x^5+240x^4+720x^3+1080x^2+810x+243$$ 7. $$(4-y)^7$$
	   <center>
<table>  
  <tr>  
    <th>1</th>  
    <th>7</th>  
    <th>21</th>  
    <th>35</th>
    <th>35</th>
    <th>21</th>
    <th>7</th>
    <th>1</th>
  </tr>  
</table>
</center>
$$\begin{align*}&1(4)^7(-y)^0+7(4)^6(-y)^1+21(4)^5(-y)^2+35(4)^4(-y)^3+\\&35(4)^3(-y)^4+21(4)^2(-y)^5+7(4)^1(-y)^6+1(4)^0(-y)^7\end{align*}$$
$$16384-2867y+21504y^2-8960y^3+2240y^4-336y^5+28y^6-y^7$$
8. $$(\frac {x}{2}+1)^5$$
   <center>
<table>  
  <tr>  
    <th>1</th>  
    <th>5</th>  
    <th>10</th>  
    <th>10</th>
    <th>5</th>
    <th>1</th>
  </tr>  
</table>
</center>
$$1(\frac{x}{2})^5(1)^0 + 5(\frac{x}{2})^4(1)^1+10(\frac{x}{2})^3(1)^2+10(\frac{x}{2})^2(1)^3+5(\frac{x}{2})^1(1)^4+1(\frac{x}{2})^0(1)^5$$
$$=\frac {x5}{32}+\frac{5x^4}{16}+\frac{5x^3}{4}+\frac{5x^2}{2}+\frac {5x}{2}+1 $$

9. $$(1-\frac{1}{x})^5$$
   <center>
<table>  
  <tr>  
    <th>1</th>  
    <th>5</th>  
    <th>10</th>  
    <th>10</th>
    <th>5</th>
    <th>1</th>
  </tr>  
</table>
</center>
$$1(1)^5(-\frac{1}{x})^0+5(1)^4(-\frac{1}{x})^1+10(1)^3(-\frac{1}{x})^2+10(1)^2(-\frac{1}{x})^3+5(1)^1(-\frac{1}{x})^4+1(1)^0(-\frac{1}{x})$$
$$=1-\frac {5}{x}+\frac {10}{x^2} - \frac {10}{x^3} + \frac {5}{x^4} - \frac {1}{x^5}$$

10. $$(2-\frac {1}{2x})^6$$
   <center>
<table>  
  <tr>  
    <th>1</th>  
    <th>6</th>  
    <th>15</th>  
    <th>20</th>
    <th>15</th>
    <th>6</th>
    <th>1</th>
  </tr>  
</table>
</center>
$$\begin{align*} &1(2)^6(-\frac{1}{2x})^0 + 6 (2)^5(-\frac{1}{2x})^1+15(2)^4(-\frac{1}{2x})^2+20(2)^3(-\frac{1}{2x})^3+\\&15(2)^2(-\frac{1}{2x})^4+6(2)^1(-\frac{1}{2x})^5+1(2)^0(-\frac{1}{2x})^6 \end{align*}$$
$$ =64-\frac{96}{x}+\frac {60}{x^2}+ \frac {20}{x^3} + \frac {15}{4x^4} - \frac {3}{8x^5} + \frac {1}{64x^6}$$

## Seatwork #4 - 2023-08-21
Find the a.) True error, b.) relative true error, c.) absolute relative true error, e.) relative approximate error of the following 

Level of tolerance $10^6$

1. The derivative of $f(x)=x^3+2x+1$ at $x=0.5$ when 
	a. $h_1 = 0.005$
	b. $h_2 = 0.001$

###### $h_1=0.005$

**True Error**
$$ f(x)=x^3+2x+1 \;, x=0.5 $$
$$f'(x)=3x^2+2$$
$$f'(x)=\lim_{h\to0} = \frac{f(x+h)-f(x)}{h}$$
$$f'(x)=\lim_{h\to0}\approx \frac{f(x+h)-f(x)}{h}\;,h=0.005\;,x=0.5$$
$$f'(x)=\lim_{h\to0}\approx \frac{f(0.5+0.005)-f(0.5)}{0.005}$$
$$f'(x)=\lim_{h\to0}\approx \frac{f(0.505)-f(0.5)}{0.005}$$
$$\approx \frac{(0.505^3+2(0.505)+1)-(0.505^3+2(0.505)+1)}{0.005}$$

$$f(0.505)=0.505^3+2(0.505)+1 = 2.138787625$$
$$f(0.5)=0.5^3+2(0.5)+1 = 2.125$$
$$\approx 2.767525$$
**Absolute Error**
$f'(x)=3x^2+2$
$$\begin{align*} \text{Absolute Error} &= | f'(x) - \frac{f(x+h)-f(x)}{h} |\\ &=|f'(0.5)-\frac{f(0.5+0.005)-f(0.5)}{0.005}|\\&=|(3(0.5)^2+2)-\frac{(0.505^3+2(0.505)+1)-(0.505^3+2(0.505)+1)}{0.005}|\end{align*}$$
$$f'(0.5) = 3(0.5)^2+2=2.75$$
$$\text{Absolute Error } = |-\frac {301}{4000}|$$
**Relative True Error**

$$\begin{align*}\text{Relative True Error}&=\frac {Absolute \; Error}{True \;Value}\\&= \frac{|(3(0.5)^2+2)-\frac{(0.505^3+2(0.505)+1)-(0.505^3+2(0.505)+1)}{0.005}|}{0.5^2+2}\end{align*}$$
$$=1$$

###### $h_2 = 0.001$
**Approximate Error**

$$\begin{align*}\text{Approx Error} &= |\frac{f(x+h_2)-f(x)}{h_2} - \frac{f(x+h_1)-f(x)}{h_1}|\\&=|\frac{f(0.5+0.001)-f(x)}{0.001} - \frac{f(0.5+0.005)-f(9.5)}{0.005}|\end{align*}$$
$$=|\frac{(0.501^3+2(0.501)+1)-(0.5^3+2(0.5)+1)}{0.001}-\frac{(0.505^3+2(0.505)+1)-(0.505^3+2(0.505)+1)}{0.005}|$$
$$f(0.501) = 0.501^3+2(0.501)+1 = 2.1277510501$$
$$f(0.5)=0.5^3+2(0.5)+1 = 2.125$$
$$=24.8392575$$

**Relative Approximate Error**

$\text{Relative Approximate Error} = \frac{|\frac{f(x+h_2)-f(x)}{h_2} - \frac{f(x+h_1)-f(x)}{h_1}|}{\frac{f(x+h_2)-f(x)}{h_2}}$
$$=\frac{|\frac{f(0.5+0.001)-f(x)}{0.001} - \frac{f(0.5+0.005)-f(9.5)}{0.005}|}{\frac{f(0.5+0.001)-f(x)}{0.001} }$$
$$=\frac{|\frac{(0.501^3+2(0.501)+1)-(0.5^3+2(0.5)+1)}{0.001}-\frac{(0.505^3+2(0.505)+1)-(0.505^3+2(0.505)+1)}{0.005}|}{\frac{(0.501^3+2(0.501)+1)-(0.5^3+2(0.5)+1)}{0.001}}$$

$$=0.902752988$$
2. The Derivative of $f(x)=(x^2+3)^3 \; at \; x=3$ when
	a. $h_1=0.01$
	b. $h_2=0.0001$

##### $h_1 = 0.01$
**True Error**

$$f(x)=(x^2+3)^3 \; at \; x=3 $$
$$f'(x) = 6x(x^2+3)^2$$
$$f'(x)=\lim_{h\to0} \frac {f(x+h)-f(x)}{h} \;, h=0.001 \;, x=3 $$
$$\approx \frac{f(3.01) - f(3)}{0.01}$$
$$f(3.01) = (3.01^2 + 3)^3 = 1754.093449$$
$$f(3) = (3^2 + 3)^3 = 1728$$
$$\approx 2609.344943$$
**Absolute Error**
$$f'(x)=6x(x^2+3)^2$$
$$\text{Absolute Error} = | f'(x) - \frac{f(x+h)-f(x)}{h} |$$
$$=|f'(3)- \frac{f(3.01) - f(3)}{0.01}|$$

$$f'(3)=6(3)((3)^2+3)^2=2592$$
$$=|-17.344944|$$
**Relative True Error**
$$=\frac{ |f'(3)- \frac{f(3.01) - f(3)}{0.01}|}{\frac{f(3.01) - f(3)}{0.01}}$$
$$=-6.69172222*10^{-03}$$

##### $h_2=0.001$
**Approximate Error**
$$Approx \; Error = |\frac{f(3.001)-f(3)}{0.001} - \frac{f(3.01) - f(3)}{0.01}|$$
$$f(3.001)=(3.001^2+3)^3 = 1730.593729$$
$$f(3)=(3^2+3)^3 = 1728$$
$$\approx -15.6129586$$
**Relative Approximate Error**
$$Relative Approx Error = \frac{|\frac{f(3.001)-f(3)}{0.001} - \frac{f(3.01) - f(3)}{0.01}|}{\frac{f(3.001)-f(3)}{0.001}}$$


$$=-5.984787178*10^{-3}$$


## Seatwork #5 - 2023-08-21
Reciprocal the following into floating point binary format given that the number is written into 10 bits. The first two bits represents the magnitude of mantissa and the remaining 3 bits represents the magnitude of the exponent.


1. 99.123

| Sign | Exponent | Mantissa | 
| --- | --- | ---|
| 00 | 101 | 11011| 
**0010111011**

2. 49.324

| Sign | Exponent | Mantissa | 
| --- | --- | ---|
| 00 | 101 | 01100 |
**0010101100**

3. -57.214

| Sign | Exponent | Mantissa | 
| --- | --- | ---|
| 10 | 101 | 10000 |
**1010110000**

4. 0.9134

| Sign | Exponent | Mantissa | 
| --- | --- | ---|
| 00 | 001 | 00011 |
**0000100011**

5. -0.6543

| Sign | Exponent | Mantissa | 
| --- | --- | ---|
| 10 | 001 | 00010 |
**1000100010**

## Seatwork #6 - 2023-08-24

Use iterative methods to solve the following 

1. $\sqrt{90}$ to 6 significant figures 
$$\sqrt{90}-9.846833$$
	$$\begin{align*}\frac{90}{10}&=9\\\frac{101.9}{2}&=9.5\\\frac{90}{9.5} &= 9.4736842\uparrow\\\frac{9.5+9.4736842}{2}&=9.4868239\\\frac{90}{9.486842105}&=9.4868239\downarrow\\\frac{9.486842105+9.48682139}{2}&=9.486833\end{align*}$$
2. $\sqrt{125}$ to 6 significant figures
$$\sqrt{125}=11.1803399$$
$$\begin{align*}\frac{125}{11}&=11.3636364\uparrow\\\frac{11+11.3636364}{2}&=11.1818182\\\frac{125}{11.1818182}&=11.1788618\downarrow\\frac{11.1818182+.1788618}{2}&=11.18033989\end{align*}$$
3. Use the iterative formula $x_{r+1}=\frac{1}{3}(2x_r + \frac{N}{x^2})$ to find the cube root of 29 to 5 significant figures 
$$\sqrt[3]{29}=3.07232$$
$$\begin{align*}\frac{29}{3.1^2}&=3.017690\downarrow\\\frac{2(3.1)+3.012690}{3}&=3.072563\\\frac{29}{3.072563^2}&=3.071825\\\frac{2(3.072563)+3.071825}{3}&=3.07232\end{align*}$$
4. Find a fraction that is within 0.000001 of the decimal 0.31245

$$\begin{align*}\frac{9}{29}\\\frac{9+11}{29+35} = &\frac
{20}{64}=0.3125\\\frac{20+9}{64+29}=&\frac{29}{93}=0.3118\\\frac{29+20}{93+64}=&\frac{49}{157}=0.31210\\\frac{49+20}{157+64}=&\frac{69}{221}=0.312217\end{align*}$$


 <center> The adding of $\frac{20}{64}$ is repeated until 0.31245 has been reached </center>
 $$....\frac{389}{1245}=0.6245$$

5. Find a fraction that is within 0.000001 of the decimal 0.552742
$$\frac{1}{2}$$
$$\begin{align*}\frac{1+1}{2+3}&=\frac{3}{5}\\\frac{3+1}{5+2}&=\frac{4}{7}\\\frac{4+1}{7+2}&=\frac{5}{9}\\\frac{5+1}{9+2}&=\frac{6}{11}\\\frac{6+5}{11+9}&=\frac{11}{20}\\\frac{11+5}{20+9}&=\frac{16}{29}\\\frac{16+5}{29+9}&=\frac{21}{38}\\\frac{21+5}{38+9}&=\frac{26}{47}\\\frac{26+21}{}\end{align*}$$

