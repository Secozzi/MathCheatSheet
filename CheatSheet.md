# Cheat Sheet

- [Cheat Sheet](#cheat-sheet)
  - [Derivatives](#derivatives)
    - [Definition](#definition)
    - [Derivative of Exponentions](#derivative-of-exponentions)
    - [Derivative of Exponentials](#derivative-of-exponentials)
    - [Derivative of Logarithms](#derivative-of-logarithms)
    - [Derivative of Trigonometric Functions](#derivative-of-trigonometric-functions)
    - [Derivative of Hyperbolic Functions](#derivative-of-hyperbolic-functions)
    - [Derivative of Inverse Trigonometric Functions](#derivative-of-inverse-trigonometric-functions)
    - [Derivative of Inverse Hyperbolic Functions](#derivative-of-inverse-hyperbolic-functions)
    - [Derivatives of Combined Functions](#derivatives-of-combined-functions)
    - [Derivatives of Special Functions](#derivatives-of-special-functions)
  - [Integrals](#integrals)
    - [Definitions](#definitions)
    - [Rules](#rules)
    - [Integrals of Rational Functions](#integrals-of-rational-functions)
    - [Integrals with Roots](#integrals-with-roots)
    - [Integrals with Logarithms](#integrals-with-logarithms)
    - [Integrals with Exponentials](#integrals-with-exponentials)
    - [Integrals with Trigonometric Functions](#integrals-with-trigonometric-functions)
    - [Products of Trigonometric Functions and Monomials](#products-of-trigonometric-functions-and-monomials)
    - [Products Of Trigonometric Functions and Exponentials](#products-of-trigonometric-functions-and-exponentials)
    - [Integrals of Hyperbolic Functions](#integrals-of-hyperbolic-functions)
  - [Trigonometric Identities](#trigonometric-identities)
    - [Radians](#radians)
    - [Pythagorean Identities](#pythagorean-identities)

## Derivatives

### Definition
$$
\frac{\partial}{\partial x} f(x) = \lim_{h \to 0} \frac{f(x+h)-f(x)}{h} \\~\\
\frac{\partial}{\partial x} f(x) = \lim_{x \to a} \frac{f(x) - f(a)}{x-a}
$$
### Derivative of Exponentions
$$
\frac{\partial}{\partial x} kx^n = nkx^{n-1} \\~\\
\frac{\partial}{\partial x} k \times f(x)^n = nk \times f(x)^{n-1} \times f'(x)
$$
### Derivative of Exponentials
$$
\frac{\partial}{\partial x} ka^x = \ln(a) \times ka^x \\~\\
\frac{\partial}{\partial x} x^{f(x)} = x^{f(x)-1} \times (x \times \ln(x) \times f'(x) + f(x)) \\~\\
\frac{\partial}{\partial x} f(x)^x = f(x)^x \times \left( \frac{x \times f'(x)}{f(x)} + \ln(f(x)) \right) \\~\\
\frac{\partial}{\partial x} f(x)^{f(x)} = f(x)^{f(x)} \times f'(x) \times (\ln(f(x))+1)
$$
### Derivative of Logarithms
$$
\frac{\partial}{\partial x} \ln(x) = \frac{1}{x}, x > 0 \\~\\
\frac{\partial}{\partial x} \ln(f(x)) = \frac{f'(x)}{f(x)} \\~\\
\frac{\partial}{\partial x} \log_a(x) = \frac{1}{x \times \ln(a)}, x > 0 \\~\\
\frac{\partial}{\partial x} \log_a(f(x)) = \frac{f'(x)}{f(x) \times \ln(a)}
$$

### Derivative of Trigonometric Functions
$$
\frac{\partial}{\partial x} \sin(x) = \cos(x) \\~\\
\frac{\partial}{\partial x} \cos(x) = -\sin(x) \\~\\
\frac{\partial}{\partial x} \tan(x) = \frac{1}{\cos^2(x)}=\sec^2(x), x\not ={\frac{\pi}{2}+\pi n, n \in \Z} \\~\\
\frac{\partial}{\partial x} \cot(x) = -\frac{1}{\sin^2(x)}=-\csc^2(x), x\not ={\pi n, n \in \Z} \\~\\
\frac{\partial}{\partial x} \sec(x) = \tan(x)\sec(x), x\not ={\frac{\pi}{2}+\pi n, n \in \Z} \\~\\
\frac{\partial}{\partial x} \csc(x) = -\cot(x)\csc(x), x\not ={\pi n, n \in \Z}
$$

### Derivative of Hyperbolic Functions
$$
\frac{\partial}{\partial x} \sinh(x) = \cosh(x) \\~\\
\frac{\partial}{\partial x} \cosh(x) = \sinh(x) \\~\\
\frac{\partial}{\partial x} \tanh(x) = \text{sech}^2(x) \\~\\
\frac{\partial}{\partial x} \text{csch}(x) = -\text{csch}(x)\coth(x), x \not ={0} \\~\\
\frac{\partial}{\partial x} \text{sech}(x) = -\text{sech}(x)\tanh(x) \\~\\
\frac{\partial}{\partial x} \coth(x) = -\text{csch}(x), x \not ={0}
$$

### Derivative of Inverse Trigonometric Functions
$$
\frac{\partial}{\partial x} \sin^{-1}(x) = \frac{1}{\sqrt{1-x^2}}, x \not ={\pm 1} \\~\\
\frac{\partial}{\partial x} \cos^{-1}(x) = \frac{-1}{\sqrt{1-x^2}}, x \not ={\pm 1} \\~\\
\frac{\partial}{\partial x} \tan^{-1}(x) = \frac{1}{1+x^2} \\~\\
\frac{\partial}{\partial x} \cot^{-1}(x) = \frac{-1}{1+x^2} \\~\\
\frac{\partial}{\partial x} \sec^{-1}(x) = \frac{1}{|x|\sqrt{x^2-1}}, x \in (-\infty, -1) \cup (1, \infty) \\~\\
\frac{\partial}{\partial x} \csc^{-1}(x) = \frac{-1}{|x|\sqrt{x^2-1}}, x \in (-\infty, -1) \cup (1, \infty)
$$

### Derivative of Inverse Hyperbolic Functions
$$
\frac{\partial}{\partial x} \sinh^{-1}(x) = \frac{1}{\sqrt{1+x^2}} \\~\\
\frac{\partial}{\partial x} \cosh^{-1}(x) = \frac{1}{\sqrt{x^2-1}}, x > 1\\~\\
\frac{\partial}{\partial x} \tanh^{-1}(x) = \frac{1}{1-x^2}, -1 < x < 1 \\~\\
\frac{\partial}{\partial x} \text{csch}^{-1}(x) = \frac{-1}{x^2\sqrt{\frac{1}{x^2}+1}}, x \not ={0} \\~\\ 
\frac{\partial}{\partial x} \text{sech}^{-1}(x) = \frac{-1}{x\sqrt{1-x^2}}, 0 < x < 1 \\~\\
\frac{\partial}{\partial x} \coth^{-1}(x) = \frac{1}{1-x^2},|x| > 1
$$

### Derivatives of Combined Functions
$$
\frac{\partial}{\partial x} f(x) \pm g(x) = f'(x) \pm g'(x) \\~\\
\frac{\partial}{\partial x} f(x) \times g(x) = f'(x) \times g(x) + f(x) \times g'(x) \\~\\
\frac{\partial}{\partial x} \frac{f(x)}{g(x)} = \frac{f'(x) \times g(x) + f(x) \times g'(x)}{g(x)^2} \\~\\
\frac{\partial}{\partial x} f(g(x)) = f'(g(x)) \times g'(x) \\~\\
\frac{\partial}{\partial x} \frac{1}{f(x)} = - \frac{f'(x)}{f(x)^2} \\~\\
\frac{f(x)}{g(x)} = \frac{f'(x)}{g'(x)}
$$

### Derivatives of Special Functions
$$
\frac{\partial}{\partial x} x! = \Gamma(x+1) \times \psi^{(0)} \times (x+1) \\~\\
\frac{\partial}{\partial z} W_n(z) = \frac{W_n(z)}{z \times W_n(z)+z} \\~\\
\frac{\partial}{\partial x} \zeta(z) = - \sum_{n=2}^\infty \frac{\ln(n)}{n^z} \\~\\
\frac{\partial}{\partial x} \text{erf}(x) = \frac{2\times e^{-x^2}}{\sqrt{\pi}}
$$

## Integrals

### Definitions
$$
\frac{d}{dx} F(x) = f(x) \\~\\
\int f(x) = F(x) \\~\\
\int_a^{b} f(x) \, dx = \big[F(x) \big]_a^b = F(b) - F(a)
$$

### Rules
$$
\int kx^{n}  = \frac{kx^{n+1}}{n+1} + C \\~\\
\int ke^{nx} = \frac{ke^{nx}}{n} + C \\~\\
\int \frac{1}{ax+b}dx = \frac{1}{a} \ln |ax + b| + C \\~\\
$$
### Integrals of Rational Functions
$$
\int \frac{1}{(x+a)^2}dx = -\frac{1}{x+a} + C \\~\\
\int (x+a)^n dx = \frac{(x+a)^{n+1}}{n+1} + C, n\ne -1\\~\\
\int x(x+a)^n dx = \frac{(x+a)^{n+1} ( (n+1)x-a)}{(n+1)(n+2)} + C\\~\\
\int \frac{1}{1+x^2}dx = \tan^{-1}(x) + C\\~\\
\int \frac{1}{a^2+x^2}dx = \frac{1}{a}\tan^{-1}(\frac{x}{a}) + C \\~\\
\int \frac{x}{a^2+x^2}dx = \frac{1}{2}\ln|a^2+x^2| + C \\~\\
\int \frac{x^2}{a^2+x^2}dx = x-a\tan^{-1}(\frac{x}{a}) + C \\~\\
\int \frac{x^3}{a^2+x^2}dx = \frac{1}{2}x^2-\frac{1}{2}a^2\ln|a^2+x^2| + C \\~\\
\int \frac{1}{ax^2+bx+c}dx = \frac{2}{\sqrt{4ac-b^2}}\tan^{-1}(\frac{2ax+b}{\sqrt{4ac-b^2}}) + C \\~\\
\int \frac{1}{(x+a)(x+b)}dx = \frac{1}{b-a}\ln\frac{a+x}{b+x} + C, \text{ } a\ne b \\~\\
\int \frac{x}{(x+a)^2}dx = \frac{a}{a+x}+\ln |a+x| + C \\~\\
\int \frac{x}{ax^2+bx+c}dx = \frac{1}{2a}\ln|ax^2+bx+c| -\frac{b}{a\sqrt{4ac-b^2}}\tan^{-1}\frac{2ax+b}{\sqrt{4ac-b^2}} + C \\~\\
$$
### Integrals with Roots
$$
\int \sqrt{x-a}\ dx = \frac{2}{3}(x-a)^{3/2} + C \\~\\
\int \frac{1}{\sqrt{x\pm a}}\ dx = 2\sqrt{x\pm a} + C \\~\\
\int \frac{1}{\sqrt{a-x}}\ dx = -2\sqrt{a-x} + C \\~\\
\int \sqrt{ax+b}\ dx = \left(\frac{2b}{3a}+\frac{2x}{3}\right)\sqrt{ax+b} + C \\~\\
\int (ax+b)^{3/2}\ dx =\frac{2}{5a}(ax+b)^{5/2} + C \\~\\
\int \frac{x}{\sqrt{x\pm a} } \ dx = \frac{2}{3}(x\mp 2a)\sqrt{x\pm a} + C \\~\\
\int \sqrt{\frac{x}{a-x}}\ dx =  -\sqrt{x(a-x)}-a\tan^{-1}\frac{\sqrt{x(a-x)}}{x-a} + C \\~\\
\int \sqrt{\frac{x}{a+x}}\ dx =  \sqrt{x(a+x)} -a\ln \left [ \sqrt{x} + \sqrt{x+a}\right] + C \\~\\
\int x \sqrt{ax + b}\ dx = \frac{2}{15 a^2}(-2b^2+abx + 3 a^2 x^2) \sqrt{ax+b} + C \\~\\
\int \sqrt{x(ax+b)}\ dx = \frac{1}{4a^{3/2}}\left[(2ax + b)\sqrt{ax(ax+b)} -b^2 \ln \left| a\sqrt{x} + \sqrt{a(ax+b)} \right| \right ] + C \\~\\
\int \sqrt{x^3(ax+b)} \ dx =\left [ \frac{b}{12a}-\frac{b^2}{8a^2x}+\frac{x}{3}\right] \sqrt{x^3(ax+b)}  + \frac{b^3}{8a^{5/2}}\ln \left | a\sqrt{x} + \sqrt{a(ax+b)} \right | + C \\~\\
\int\sqrt{x^2 \pm a^2}\ dx = \frac{1}{2}x\sqrt{x^2\pm a^2} \pm\frac{1}{2}a^2 \ln \left | x + \sqrt{x^2\pm a^2} \right | + C \\~\\
\int  \sqrt{a^2 - x^2}\ dx = \frac{1}{2} x \sqrt{a^2-x^2} +\frac{1}{2}a^2\tan^{-1}\frac{x}{\sqrt{a^2-x^2}} + C \\~\\
\int  x \sqrt{x^2 \pm a^2}\ dx= \frac{1}{3}\left ( x^2 \pm a^2 \right)^{3/2} + C \\~\\
\int \frac{1}{\sqrt{x^2 \pm a^2}}\ dx = \ln \left | x + \sqrt{x^2 \pm a^2}\right | + C \\~\\
\int \frac{1}{\sqrt{a^2 - x^2}}\ dx = \sin^{-1}\frac{x}{a} + C \\~\\
\int \frac{x}{\sqrt{x^2\pm a^2}}\ dx = \sqrt{x^2 \pm a^2} + C \\~\\
\int \frac{x}{\sqrt{a^2-x^2}}\ dx = -\sqrt{a^2-x^2} + C \\~\\
\int \frac{x^2}{\sqrt{x^2 \pm a^2}}\ dx = \frac{1}{2}x\sqrt{x^2 \pm a^2} \mp \frac{1}{2}a^2 \ln \left| x + \sqrt{x^2\pm a^2} \right | + C \\~\\
\int \sqrt{a x^2 + b x + c}\ dx = \frac{b+2ax}{4a}\sqrt{ax^2+bx+c} + \frac{4ac-b^2}{8a^{3/2}}\ln \left| 2ax + b + 2\sqrt{a(ax^2+bx^+c)}\right | + C \\~\\
\int\frac{1}{\sqrt{ax^2+bx+c}}\ dx = \frac{1}{\sqrt{a}}\ln \left| 2ax+b + 2 \sqrt{a(ax^2+bx+c)} \right | + C \\~\\
\int \frac{x}{\sqrt{ax^2+bx+c}}\ dx=\frac{1}{a}\sqrt{ax^2+bx + c} -\frac{b}{2a^{3/2}}\ln \left| 2ax+b + 2 \sqrt{a(ax^2+bx+c)} \right | + C \\~\\
\int\frac{dx}{(a^2+x^2)^{3/2}}=\frac{x}{a^2\sqrt{a^2+x^2}} + C \\~\\
$$
### Integrals with Logarithms
$$
\int \ln ax\  dx = x \ln ax - x + C \\~\\
\int x \ln x \ dx = \frac{1}{2} x^2 \ln x-\frac{x^2}{4} + C \\~\\
\int x^2 \ln x \ dx = \frac{1}{3} x^3 \ln x-\frac{x^3}{9} + C \\~\\
\int x^n \ln x\ dx = x^{n+1}\left( \dfrac{\ln x}{n+1}-\dfrac{1}{(n+1)^2}\right) + C,\hspace{2ex} n\neq -1 \\~\\
\int \frac{\ln ax}{x}\ dx = \frac{1}{2}\left ( \ln ax \right)^2 + C \\~\\
\int \frac{\ln x}{x^2}\ dx = -\frac{1}{x}-\frac{\ln x}{x} + C \\~\\
\int \ln (ax + b) \ dx = \left ( x + \frac{b}{a} \right) \ln (ax+b) - x + C, a\ne 0 \\~\\
\int \ln  ( x^2 + a^2 )\hspace{.5ex} {dx} = x \ln (x^2 + a^2  ) +2a\tan^{-1} \frac{x}{a} - 2x + C \\~\\
\int \ln  ( x^2 - a^2 )\hspace{.5ex} {dx} = x \ln (x^2 - a^2  ) +a\ln \frac{x+a}{x-a} - 2x + C \\~\\
\int \ln \left ( ax^2 + bx + c\right) \ dx  = \frac{1}{a}\sqrt{4ac-b^2}\tan^{-1}\frac{2ax+b}{\sqrt{4ac-b^2}} -2x + \left( \frac{b}{2a}+x \right )\ln \left (ax^2+bx+c \right) + C \\~\\
\int x \ln (ax + b)\ dx = \frac{bx}{2a}-\frac{1}{4}x^2 +\frac{1}{2}\left(x^2-\frac{b^2}{a^2}\right)\ln (ax+b) + C \\~\\
\int x \ln \left ( a^2 - b^2 x^2 \right )\ dx = -\frac{1}{2}x^2+ \frac{1}{2}\left( x^2 - \frac{a^2}{b^2} \right ) \ln \left (a^2 -b^2 x^2 \right) + C \\~\\
\int (\ln x)^2\ dx = 2x - 2x \ln x + x (\ln x)^2 + C \\~\\
\int (\ln x)^3\ dx = -6 x+x (\ln x)^3-3 x (\ln x)^2+6 x \ln x + C \\~\\
\int x (\ln x)^2\ dx = \frac{x^2}{4}+\frac{1}{2} x^2 (\ln x)^2-\frac{1}{2} x^2 \ln x + C \\~\\
\int x^2 (\ln x)^2\ dx = \frac{2 x^3}{27}+\frac{1}{3} x^3 (\ln x)^2-\frac{2}{9} x^3 \ln x + C \\~\\
$$
### Integrals with Exponentials
$$
\int e^{ax}\ dx = \frac{1}{a}e^{ax} + C \\~\\
\int \sqrt{x} e^{ax}\ dx = \frac{1}{a}\sqrt{x}e^{ax} +\frac{i\sqrt{\pi}}{2a^{3/2}} \text{erf}\left(i\sqrt{ax}\right) + C, \text{ where erf}(x)=\frac{2}{\sqrt{\pi}}\int_0^x e^{-t^2}dt \\~\\
\int x e^x\ dx = (x-1) e^x + C \\~\\
\int x e^{ax}\ dx = \left(\frac{x}{a}-\frac{1}{a^2}\right) e^{ax} + C \\~\\
\int x^2 e^{x}\ dx = \left(x^2 - 2x + 2\right) e^{x} + C \\~\\
\int x^2 e^{ax}\ dx = \left(\frac{x^2}{a}-\frac{2x}{a^2}+\frac{2}{a^3}\right) e^{ax} + C \\~\\
\int x^3 e^{x}\ dx = \left(x^3-3x^2 + 6x - 6\right) e^{x} + C \\~\\
\int x^n e^{ax}\ dx = \frac{x^{n}(-ax)^{-n}\Gamma (n+1, -ax)}{a}+C, \text{where }\Gamma (a, x) =\int_x^{\infty} t^{a-1}e^{-t}\hspace{2pt}\text{d}t \\~\\
\int e^{ax^2}\ dx = -\frac{i\sqrt{\pi}}{2\sqrt{a}}\text{erf}\left(ix\sqrt{a}\right) + C \\~\\
\int e^{-ax^2}\ dx = \frac{\sqrt{\pi}}{2\sqrt{a}}\text{erf}\left(x\sqrt{a}\right) + C \\~\\
\int x e^{-ax^2}\ {dx} = -\dfrac{1}{2a}e^{-ax^2} + C \\~\\
\int x^2 e^{-ax^2}\ {dx} = \dfrac{1}{4}\sqrt{\dfrac{\pi}{a^3}}\text{erf}(x\sqrt{a}) -\dfrac{x}{2a}e^{-ax^2} + C \\~\\
$$
### Integrals with Trigonometric Functions
$$
\int \sin ax \ dx = -\frac{1}{a} \cos ax + C \\~\\
\int \sin^2 ax\  dx = \frac{x}{2} - \frac{\sin 2ax} {4a} + C \\~\\
\int \sin^3 ax \ dx = -\frac{3 \cos ax}{4a} + \frac{\cos 3ax} {12a} + C \\~\\
\int \sin^n ax \ dx = -\frac{1}{a}{\cos ax} \hspace{0.5mm}{_2F_1}\left[ \frac{1}{2}, \frac{1-n}{2}, \frac{3}{2}, \cos^2 ax \right] + C \\~\\
\int \cos ax\ dx= \frac{1}{a} \sin ax + C \\~\\
\int \cos^2 ax\ dx = \frac{x}{2}+\frac{ \sin 2ax}{4a} + C \\~\\
\int \cos^3 ax dx = \frac{3 \sin ax}{4a}+\frac{ \sin 3ax}{12a} + C \\~\\
\int \cos^p ax dx  = -\frac{1}{a(1+p)}{\cos^{1+p} ax} \times {_2F_1}\left[ \frac{1+p}{2}, \frac{1}{2}, \frac{3+p}{2}, \cos^2 ax \right] + C \\~\\
\int \cos x \sin x\ dx = \frac{1}{2}\sin^2 x + c_1 = -\frac{1}{2} \cos^2x + c_2 = -\frac{1}{4} \cos 2x + c_3 \\~\\
\int \cos ax \sin bx\ dx = \frac{\cos[(a-b) x]}{2(a-b)} - \frac{\cos[(a+b)x]}{2(a+b)} + C, a\ne b \\~\\
\int \sin^2 ax \cos bx\ dx = -\frac{\sin[(2a-b)x]}{4(2a-b)} + \frac{\sin bx}{2b} - \frac{\sin[(2a+b)x]}{4(2a+b)} + C \\~\\
\int \sin^2 x \cos x\ dx = \frac{1}{3} \sin^3 x + C \\~\\
\int \cos^2 ax \sin bx\ dx = \frac{\cos[(2a-b)x]}{4(2a-b)} - \frac{\cos bx}{2b} - \frac{\cos[(2a+b)x]}{4(2a+b)} + C \\~\\
\int \cos^2 ax \sin ax\ dx = -\frac{1}{3a}\cos^3{ax} + C \\~\\
\int \sin^2 ax \cos^2 bx dx = \frac{x}{4} -\frac{\sin 2ax}{8a}- \frac{\sin[2(a-b)x]}{16(a-b)} +\frac{\sin 2bx}{8b}- \frac{\sin[2(a+b)x]}{16(a+b)} + C \\~\\
\int \sin^2 ax \cos^2 ax\ dx = \frac{x}{8}-\frac{\sin 4ax}{32a} + C \\~\\
\int \tan ax\ dx = -\frac{1}{a} \ln \cos ax + C \\~\\
\int \tan^2 ax\ dx = -x + \frac{1}{a} \tan ax + C \\~\\
\int \tan^n ax\ dx = \frac{\tan^{n+1} ax }{a(1+n)} \times {_2}F_1\left( \frac{n+1}{2}, 1, \frac{n+3}{2}, -\tan^2 ax \right) + C \\~\\
\int \tan^3 ax dx = \frac{1}{a} \ln \cos ax + \frac{1}{2a}\sec^2 ax + C \\~\\
\int \sec x \ dx = \ln | \sec x + \tan x | = 2 \tanh^{-1} \left (\tan \frac{x}{2} \right) + C \\~\\
\int \sec^2 ax\ dx = \frac{1}{a} \tan ax + C \\~\\ 
\int \sec^3 x \ {dx} = \frac{1}{2} \sec x \tan x + \frac{1}{2}\ln | \sec x + \tan x | + C \\~\\
\int \sec x \tan x\ dx = \sec x + C \\~\\
\int \sec^2 x \tan x\ dx = \frac{1}{2} \sec^2 x + C \\~\\
\int \sec^n x \tan x \ dx = \frac{1}{n} \sec^n x + C, n\ne 0 \\~\\
\int \csc x\ dx = \ln \left | \tan \frac{x}{2} \right|  = \ln | \csc x - \cot x| + C \\~\\
\int \csc^2 ax\ dx = -\frac{1}{a} \cot ax + C \\~\\
\int \csc^3 x\ dx = -\frac{1}{2}\cot x \csc x + \frac{1}{2} \ln | \csc x - \cot x | + C \\~\\
\int \csc^nx \cot x\ dx = -\frac{1}{n}\csc^n x + C, n\ne 0 \\~\\
\int \sec x \csc x \ dx = \ln | \tan x | + C \\~\\
$$
### Products of Trigonometric Functions and Monomials
$$
\int x \cos x \ dx = \cos x + x \sin x + C \\~\\
\int x \cos ax \ dx = \frac{1}{a^2} \cos ax + \frac{x}{a} \sin ax + C \\~\\
\int x^2 \cos x \ dx = 2 x \cos x + \left ( x^2 - 2 \right ) \sin x + C \\~\\
\int x^2 \cos ax \ dx = \frac{2 x \cos ax }{a^2} + \frac{ a^2 x^2 - 2  }{a^3} \sin ax + C \\~\\
\int  x^n \cos x dx = \frac{1}{2}ix^n(x^2)^{-n}\left( (-ix)^n\Gamma (n+1, ix)-(ix)^n\Gamma (n+1, -ix) \right) + C \\~\\
\int x \sin x\ dx = -x \cos x + \sin x + C \\~\\
\int x \sin ax\ dx = -\frac{x \cos ax}{a} + \frac{\sin ax}{a^2} + C \\~\\
\int x^2 \sin x\ dx = \left(2-x^2\right) \cos x + 2 x \sin x + C \\~\\
\int x^2 \sin ax\ dx =\frac{2-a^2x^2}{a^3}\cos ax +\frac{ 2 x \sin ax}{a^2} + C \\~\\
\int x \cos^2 x \ dx = \frac{x^2}{4}+\frac{1}{8}\cos 2x + \frac{1}{4} x \sin 2x + C \\~\\
\int x \sin^2 x \ dx = \frac{x^2}{4}-\frac{1}{8}\cos 2x - \frac{1}{4} x \sin 2x + C \\~\\
\int x \tan^2 x \ dx = -\frac{x^2}{2} + \ln \cos x + x \tan x + C \\~\\
\int x \sec^2 x \ dx = \ln \cos x + x \tan x + C \\~\\
$$
### Products Of Trigonometric Functions and Exponentials
$$
\int e^x \sin x \ dx = \frac{1}{2}e^x (\sin x - \cos x) + C \\~\\
\int e^{bx} \sin ax\ dx = \frac{1}{a^2+b^2}e^{bx} (b\sin ax - a\cos ax) + C \\~\\
\int e^x \cos x\ dx = \frac{1}{2}e^x (\sin x + \cos x) + C \\~\\
\int e^{bx} \cos ax\ dx = \frac{1}{a^2 + b^2} e^{bx} ( a \sin ax + b \cos ax ) + C \\~\\
\int x e^x \sin x\ dx = \frac{1}{2}e^x (\cos x - x \cos x + x \sin x) + C \\~\\
\int x e^x \cos x\ dx = \frac{1}{2}e^x (x \cos x - \sin x + x \sin x) + C \\~\\
$$
### Integrals of Hyperbolic Functions
$$
\int \cosh ax\ dx =\frac{1}{a} \sinh ax + C \\~\\
\int e^{ax}  \cosh bx \ dx = \begin{cases} \displaystyle{\frac{e^{ax}}{a^2-b^2} }[ a \cosh bx - b \sinh bx ] + C & a\ne b \\ \displaystyle{\frac{e^{2ax}}{4a} + \frac{x}{2}} + C & a = b \end{cases} \\~\\
\int \sinh ax\ dx = \frac{1}{a} \cosh ax + C \\~\\
\int e^{ax} \sinh bx \ dx =\begin{cases} \displaystyle{\frac{e^{ax}}{a^2-b^2} }[ -b \cosh bx + a \sinh bx ] + C & a\ne b \\ \displaystyle{\frac{e^{2ax}}{4a} - \frac{x}{2}} + C & a = b \end{cases} \\~\\
\int \tanh ax\hspace{1.5pt} dx =\frac{1}{a} \ln \cosh ax + C \\~\\
\int  e^{ax} \tanh bx\ dx = \begin{cases} \displaystyle{ \frac{ e^{(a+2b)x}}{(a+2b)} {_2F_1}\left[ 1+\frac{a}{2b},1,2+\frac{a}{2b}, -e^{2bx}\right] } + C& \\ \displaystyle{\hspace{1cm}-\frac{1}{a}e^{ax}{_2F_1}\left[ 1, \frac{a}{2b},1+\frac{a}{2b}, -e^{2bx}\right]} + C& a\ne b \\ \displaystyle{\frac{e^{ax}-2\tan^{-1}[e^{ax}]}{a} } + C& a = b \end{cases} \\~\\
\int \cos ax \cosh bx\ dx = \frac{1}{a^2 + b^2} \left[a \sin ax \cosh bx  + b \cos ax \sinh bx \right] + C \\~\\
\int \cos ax \sinh bx\ dx = \frac{1}{a^2 + b^2} \left[b \cos ax \cosh bx + a \sin ax \sinh bx \right] + C \\~\\
\int \sin ax \cosh bx \ dx = \frac{1}{a^2 + b^2} \left[-a \cos ax \cosh bx + b \sin ax \sinh bx \right] + C \\~\\
\int \sin ax \sinh bx \ dx = \frac{1}{a^2 + b^2} \left[b \cosh bx \sin ax - a \cos ax \sinh bx \right] + C \\~\\
\int \sinh ax \cosh ax dx= \frac{1}{4a}\left[ -2ax + \sinh 2ax \right] + C \\~\\
\int \sinh ax \cosh bx \ dx = \frac{1}{b^2-a^2}\left[ b \cosh bx \sinh ax - a \cosh ax \sinh bx \right] + C
$$


## Trigonometric Identities

### Radians
$1^{\circ} = \frac{\pi}{180} \text{rad, 1 rad}=\frac{180^{\circ}}{\pi}\approx 57,3^{\circ}$

### Pythagorean Identities
$$
\sin^2(\theta) + \cos^2(\theta) = 1 \\~\\
\sec^2(\theta) = 1 + \tan^2(\theta) \\~\\
\csc^2(\theta) = 1 + \cot^2(\theta) \\~\\
$$

| in terms of | $\sin(\theta)$ | $\cos(\theta)$ | $\tan(\theta)$ | $\csc(\theta)$ | $\sec(\theta)$ | $\cot(\theta)$ |
|---|---|---|---|---|---|---|
| $\sin(\theta)=$ | $\sin(\theta)$ | $\pm \sqrt{1-\cos^2(\theta)}$ | $\pm \frac{\tan{\theta}}{\sqrt{1+\tan^2(\theta)}}$ | $\frac{1}{\csc(\theta)}$ | $\pm \frac{\sqrt{\sec^2(\theta)-1}}{\sec(\theta)}$ | $\pm \frac{1}{\sqrt{1+\cot^2(\theta)}}$ |
| $\cos(\theta)=$ | $\pm \sqrt{1-\sin^2(\theta)}$ | $\cos(\theta)$ | $\pm \frac{1}{\sqrt{1+\tan^2(\theta)}}$ | $\pm \frac{\sqrt{\csc^2(\theta)-1}}{\csc(\theta)}$ | $\frac{1}{\sec(\theta)}$ | $\pm \frac{\cot{\theta}}{\sqrt{1+\cot^2(\theta)}}$ |
| $\tan(\theta)=$ | $\pm \frac{\sin{\theta}}{\sqrt{1-\sin^2(\theta)}}$ | $\pm \frac{\sqrt{1-\cos^2(\theta)}}{\cos(\theta)}$ | $\tan(\theta)$ | $\pm \frac{1}{\sqrt{\csc^2(\theta)-1}}$ | $\pm \sqrt{\sec^2(\theta)-1}$ | $\frac{1}{\cot(\theta)}$ |
| $\csc(\theta)=$ | $\frac{1}{\sin(\theta)}$ | $\pm \frac{1}{\sqrt{1-\cos^2(\theta)}}$ | $\pm \frac{\sqrt{1+\tan^2(\theta)}}{\tan(\theta)}$ | $\csc(\theta)$ | $\pm \frac{\sec{\theta}}{\sqrt{\sec^2(\theta)-1}}$ | $\pm \sqrt{1+\cot^2(\theta)}$ |
| $\sec(\theta)=$ | $\pm \frac{1}{\sqrt{1-\sin^2(\theta)}}$ | $\frac{1}{\cos(\theta)}$ | $\pm \sqrt{1+\tan^2(\theta)}$ | $\pm \frac{\csc{\theta}}{\sqrt{\csc^2(\theta)-1}}$ | $\sec(\theta)$ | $\pm \frac{\sqrt{1+\cot^2(\theta)}}{\cot(\theta)}$ |
| $\cot(\theta)=$ | $\pm \frac{\sqrt{1-\sin^2(\theta)}}{\sin(\theta)}$ | $\pm \frac{\cos{\theta}}{\sqrt{1-\cos^2(\theta)}}$ | $\frac{1}{\tan(\theta)}$ | $\pm \sqrt{\csc^2(\theta)-1}$ | $\pm \frac{1}{\sqrt{\sec^2(\theta)-1}}$ | $\cot(\theta)$ |

<style>th,td{border: 1px solid white}table{margin-left:auto;margin-right:auto}</style>