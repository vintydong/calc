<link rel=stylesheet href="./style.css">
<div id="container">

# AP Calculus Cheat Sheet
=====================================================================

Table of Contents

[Unit 1](#unit-1-3) <br>
[Unit 2](#unit-2-3) <br>
[Unit 3](#unit-3-3) <br>
[Unit 4 - Integration](#unit-4---integration-3) <br>
[Unit 6 - Differential Equations](#unit-6-differential-equations-3) <br>
[Unit 7 - Area and Volume](#unit-7-area-and-volume-3) <br>
[Formulas](#formulas-3) <br>

=====================================================================

## Unit 1
**Defintion of a Limit** 

$$ \lim\limits_{x \to a-}  = \lim\limits_{x \to a+} = \lim\limits_{x \to a} = L $$

* A limit exists if the left-handed and right-handed limits are the same & $L$ is a real number (not $\infty$)

**Definition of Continuity** 

* A function is continuous at $a$ if $f(a) = \lim_{x \to a}f(x)$

* $f(x)$ is a continuous function if this is true for all values in the domain

**Properties of Limits**

$$ Let \; b \; and \; c \; be \; real \; numbers, \; let \; n \; be \; a \; positive \; integer, \; 
\newline and \; let \; f \; and \; g \; be \; functions \; with \; the \; following \; limits: 
\newline \lim\limits_{x \to c} f(x) = L \quad and \quad \lim\limits_{x \to c} g(x) = K
$$

1. Scalar Multiple: $\lim_{x \to c} \; b\,f(x) = b \, L$
2. Sum/Difference: $\lim_{x \to c} \; [f(x) \pm g(x)] = L \pm K$
3. Product: $\lim_{x \to c} \; [f(x) \, g(x)] = L \, K$
4. Quotient: $\lim_{x \to c} \frac{f(x)}{g(x)} = \frac{L}{K}, K \ne 0$
5. Power: $\lim_{x \to c} \; [f(x)]^n = L^n$

**Squeeze Theorem**

$$ 
Let \; f, \; g, \; and \; h \; be \; functions \; defined \; on \; an \; interval \; I, such \; that \; g(x) \le f(x) \le h(x) \; for \; x \ne a.
\newline
Suppose \lim_{x \to a} g(x) = \lim_{x \to a} h(x) = L, 
\newline
then, \lim_{x \to a} f(x) = L.
$$

**Intermediate Value Theorem**

If $f$ is continuous on the *closed* interval $[a,b]$, and $f(a) \ne f(b)$, and $k$ is a number between $f(a)$ and $f(b)$, then there exists at least a number $c$ in $(a,b)$, such that $f(c) = k$.

* $f(x)$ *must* be continuous on the interval
* For justification, mention that $f(x)$ is continuous over the interval.
    * Ex: Since $f(x)$ is continuous over $[a,b]$, and $f(a) \lt 2 \lt f(b)$, there is a $c$ in $(a,b)$ such that $f(c) = 2$.

**L'Hopital's Rule**

If $\lim_{x \to c} f(x) = \lim_{x \to c} g(x) = 0$ or $\pm \infty$, then

$$
    \lim_{x \to c} \frac{f(x)}{g(x)} = \lim_{x \to c} \frac{f'(x)}{g'(x)}
$$

---
## Unit 2
**Definition of Derivative:**

$$
\frac{dy}{dx} = f'(x) = \lim\limits_{h \to 0} \; \frac{f(x+h)-f(x)}{h}
$$
Alternate Form:

$$
\frac{dy}{dx} = f'(x) = \lim\limits_{x \to a} \; \frac{f(x)-f(a)}{x-a}
$$
* The derivative at $x=a$ is the instantaneous rate of change at that point.
* The derivative at $x=a$ is the slope of the tangent line at that point.

Tangent Line: 

$$y - f(a) = f'(a)(x-a)$$

A horizontal tangent exists when $\frac{dy}{dx} = f'(x) = 0$ 
<br>
A vertical tangent exists when $\frac{dy}{dx} = f'(x) = undefined$

* Undefined refers to a division by zero. 

**Differentiability**
* A derivative exists at $x=c$ if  

$$
\lim_{h \to 0-} \frac{f(x+h)-f(x)}{h} = \lim_{h \to 0+} \frac{f(x+h)-f(x)}{h}
$$
* A function is differentiable at $x=c$ if the derivative exists at $x=c$. 
* A function is differentiable on an open interval $(a,b)$ if it's differentiable at every point in the interval.
* <u>Note:</u> The derivative exists at a point if the slope from the left side is equal to the slope from the right side
* <u>Note:</u> If a function is differentiable on an open interval, it is also continuous over the same interval. That is, differentiability guarantees continuity. (Continuity does **not** guarantee differentiability). <br>
The graph of $f(x) = |x|$ is continuous over $(-1,1)$ but is not differentiable at $x=0$ because the derivative from the left ($-1$) does not equal the derivative from the right $(1)$.

To be differentiable, a function must be continuous and fulfill the above requirements.

---
## Unit 3

**Extreme Value Theorem**

If $f(x)$ is continuous on a closed interval $[a,b]$, then $f$ must attain a maximum and a minimum, each at least once.

**Critical Point**

$f'(c)$ is a critical point of $f$ if $f'(c) = 0$ or $f'(c) = undefined$

**First Derivative Test**

$f(x)$ will have a relative max when $f'(x)$ switches from **positive** to **negative** around a critical point.

$f(x)$ will have a relative min when $f'(x)$ switches from **negative** to **positive** around a critical point.

* Relative extremas are greater/less than their surround points. 
* Endpoints are **not** relative extremas. There are no points on one side of the endpoint.
* To find relative extremas, find all critical points $c$ and check if $f'$ changes signs around point $c$.

**Concavity** 

A function *f* is concave up when the slope increases. The rate of change of the function is increasing. The graph opens up.

* $f''(x) > 0$

A function *f* is concave down when the slope decreases. The rate of change of the function is decreasing. The graph opens up.

* $f''(x) < 0$

**Inflection Point** 

A point *c* is an inflection point if the graph of $f$ changes concavity around $x=c$. 

$$f''(c) = 0$$

* $f''(c)$ has to change signs around $c$.

**Second Derivative Test**

A critical point $c$ is a relative max if $f''(c) < 0$.

A critical point $c$ is a relative min if $f''(c) > 0$.

* If the graph was concave up around a critical point, then the slope is increasing, therefore $f'(x)$ is going from negative to positive.
* If the graph was concave down around a critical point, then the slope is decreasing, therefore $f'(x)$ is going from positive to negative.

**Mean Value Theorem**

If $f$ is a continuous function on the closed interval $[a,b]$ and differentiable on the open interval $(a,b)$, then there exists a point $c$ in $(a,b)$ such that 

$$f'(c) = \frac{f(b)-f(a)}{b-a}$$

* The MVT **requires** the function be continuous and differentiable. 
    * $f$ is only differentiable at an open interval because it is possible the endpoints to not be differentiable. 
* The theorem can be restated as the secant between two points is parallel to a tangent line within the interval.
* For questions asking for a justification of the MVT, it must be stated that the function is differentiable.
    * Ex: Since $f$ is differentiable over $(a,b)$, by the MVT, there is some $c$ in $(a,b)$ where $f'(c) = \frac{f(b)-f(a)}{b-a}$.
* **Rolle's Theorem** is a special case of the MVT where $f'(c)$ = 0.

| $f(x)$ | $f'(x)$ | $f''(x)$ | Note |
|:---:|:---:|:---:|:---:|
Increasing| >0 |  |
Decreasing| <0 |  |
Concave Up| Increasing | >0 |
Concave Down| Decreasing | <0 |
|| Increasing | >0 |

<br>

|  |0|
|:---:|:---:|
|$f$ | Root of $f$|
|$f'$| Critical point <br> Possible relative extrema|
|$f''$| Possible point of inflection |

**Linearization and Linear Approximation** 

Using the tangent line at $x=a$ to approximate values of x:

$$
y- f(a) = f'(a) \, (x-a)
\newline
f(x) \approx f'(a) \, (x-a) + f(a)
$$

* Since it is an approximation, do not write $=$ and use $\approx$

**Derivative of Inverse Functions**

$$
    (f^{-1})^{'}(x) = \frac{1}{f'(f^{-1}(x))}
$$
* For a point $(x,y)$ where $y=f(x)$, the corresponding point of the inverse function $f^{-1}(x)$ is $(y,x)$.
* Following the formula, the derivative of $f^{-1}(x)$ at $(y,x)$ is $\frac{1}{f'(y)}$.
1. If given $f(x)$ or a table of points and asked to find the derivative of the inverse function, first determine the point.
2. If asked to find the derivative of the inverse at $x=a$, then find the $x$-value at which the *original* function is equal to $a$. Substitute the quantities into the equation above. This means you will need the derivative of the original equation or a table of values for $f'$.

**Notes**

* To find relative extremas, either the First Derivative Test or the Second Derivative can be used. One may be easier than the other. 
* For questions asking whether a point is a relative extrema, justify by stating how the sign of $f'(x)$ changes (from positive to negative or vice versa).
* For any relative extreme or inflection point problem, do not forget that $\frac{dy}{dx}$ and $\frac{d^2y}{dx^2}$ respectively, could equal to undefined; it just needs to change signs. 

---
## Unit 4 - Integration

**Antiderivative or Indefinite Integral**

A function $y=f(x)$ is an antiderivative or an indefinite integral of $\frac{dy}{dx} = f'(x)$

* The terms antiderivative and indefinite integral are interchangeable and both refer to the general equation that is the solution to an integral. 
* Whenever an indefinite integral is taken, there is a constant of integration $c$, added to the equation.

**Integration by Substitution (u-sub)**

Conditions for using u-sub 
* There must a constant multiple of the derivative of the function being substituted
* The resulting integral is something that can be evaluated.

$$
\int f(x) \, f'(x) \, dx \quad u=f(x)
\newline
\int u \, du \quad\quad du = f'(x) \, dx
\newline
= \frac{u^2}{2}+c
\newline
= \frac{f(x)^2}{2} + c
$$

* Think of u-sub as undoing the chain rule.
* After u-sub, all the terms in the integral should be in terms of u.
* Remember to change $dx$ into $du$ correctly.

**Riemann Sums and Summations**

Used for approximating the area under a curve by breaking the graph into intervals where each interval is a rectangle.

* Right Riemann Sums - uses the right value of the sub-interval 
    * $f(b) * (b-a)$
    * Overapproximates for increasing functions
    * Underapproximates for decreasing functions
* Left Riemann Sums - uses the left value of the sub-interval 
    * $f(a) * (b-a)$
    * Overapproximates for decreasing functions
    * Underapproximates for increasing functions
* Midpoint Riemann Sums - uses the midpoint value of the sub-interval 
    * $f(\frac{a+b}{2}) * (b-a)$
    * Overapproximates for concave down
    * Underapproximates for concave up
* Trapezoidal Riemann Sums - uses the average value of the sub-interval 
    * $\frac{f(a)+f(b)}{2} * (b-a)$
    * Overapproximates for concave up
    * Underapproximates for concave down

Riemann Sums can be expressed as a summation of $n$ sub-intervals.

$$
\sum_{i=0}^{n}f_{i} \, x_{i}
$$

As the $lim_{n \to \infty}$ of the summation, it becomes the summation representation of the integral.

$$
\lim_{n \to \infty} \sum_{i=0}^{n}f_{i} \, x_{i}
$$

$$
\int_a^b f(x) \, dx = \lim_{n \to \infty} \sum_{k=0}^{n}[ f(a+\frac{k(b-a)}{n}) \, \frac{b-a}{n} ]
$$

* $\frac{b-a}{n}$ is the term that becomes $dx$ as $\lim_{n \to \infty}$
    * It is also the length of the equal sub-intervals.
* The $f(a+\frac{k(b-a)}{n})$ term is equal to $f(a)$ when $k=0$.
* As $\lim_{n \to \infty}$ and $k \to n$, the $f(a+\frac{k(b-a)}{n})$ term in the summation will be equal to $f(b)$.

**Definite Integral**

$$
\int_a^b f(x) \, dx
$$

The definite integral gives a value unlike the indefinite integral that gives a general equation. The value is equal to the area under the curve of $f(x)$ from $x=a$ to $x=b$.

* The value that the definite integral evaluates to is also know as the net change of the antiderivative from $x=a$ to $x=b$.
* A definite integral is evaluated by finding the indefinite integral and applying the following theorem

**Fundamental Theorem of Calculus**

$$
Let \; F(x) \; be \; the \; antiderivative \; of \; f(x).
\newline
\int_a^b f(x) \, dx = F(b) - F(a)
$$

**Integral Defined Functions**

Integral defined functions are functions that are defined by the integration of another function.

$$
g(x) = \int_a^x f(t) \, dt
$$

**Second Fundamental Theorem of Calculus**

$$
\frac{d}{dx} \, g(x) = \frac{d}{dx} \, \int_a^x f(t) \, dt = f(x)
\newline
g'(x)=f(x)
$$

* The upper limit of integration is a function
* The lower limit of integration is a constant
* In cases where upper limit is a constant and the lower is a function, flip the integral first.

**Average Value of a Function**

The average value of a function $f$ over an interval $[a,b]$ is 

$$
\frac{1}{b-a} \, \int_a^b f(x) \, dx
$$

Can be rewritten as 

$$
    \frac{F(b)-F(a)}{b-a}
$$

**MVT for Integrals**

$$
Let \; F(x) \; be \; the \; antiderivative \; of \; f(x), \; the \; MVT \; guarantees \;
\newline
F'(c)=f(c)=\frac{F(B)-F(a)}{b-a}
$$
* $F(b) - F(a)$ is the net change over $[a,b]$
* This means that the average value of the function is the average rate of change of the antiderivative.
    * The slope of the line from $(a,F(a))$ to $(b, F(b))$ is the average value of $f(x)$.

**Notes**
* Integrals begin with the integral symbol with either two limits of integration (an upper and lower) or none (for indefinite integrals). The expression that is being integrated (the integrand) ends with the differential (dx).
---
## Unit 6: Differential Equations

A differential equation is an equation that involves at least 1 derivative

A solution to a differential equation is any function that satisfies the equation.

The paricular solution of a differential equation is the original function in the form of $y=f(x)$ that contains a specific point, referred to as the initial condition.

The domain of the particular solution is the interval over which $f(x)$ is defined, differentiable, and contains the initial condition. 

**Separable Differential Equation** 

A differential equation that can be written with each of the 2 variables on a different side of the equation. 
1. Separation of variables is rewriting the equation such that the y terms are on one side and the x terms on the other (including $dy$ and $dx$).
2. Integrate both sides with the constant of integration, $c$, on the side with the x terms.
3. For particular solutions, $c$ needs to found.
4. Solve for $y$ to find the solution to the differential equation.

**Slope Fields**

Short line segments with slope $\frac{dy}{dx}$ at $(x,y)$, form a slope field and shows the general shape of all solutions of $\frac{dy}{dx} = f(x)$.


To match slope fields with the correct $\frac{dy}{dx}$ equation, look at the equation.
1. If $\frac{dy}{dx}$ only contains either $x$ or $y$, then it will only change as that variable is changed. 
    * Ex: $\frac{dy}{dx} = x^2$ will only change with x so all line segments on $x=2$ will be the same.
2. $\frac{dy}{dx}$ may contain a variable raised to an even power. This variable will not change the sign of the slope.
    * Ex: $\frac{dy}{dx} = \frac{x}{y^2}$ Since $y$ is squared, then the slopes should be negative when $x$ is negative and vice versa. 
3. Notice places where $\frac{dy}{dx}$ is either 0 or undefined. That is the slope is either horizontal or vertical. If the slopes along a given $x$ or $y$ is horizontal/vertical, that should be a factor in the differential equation.
    * Ex: All the slopes along $y=2$ is horizontal and vertical along $x=1$. This means the differential equation should have $(y-2)$ in the numerator and $(x-1)$ in the denominator.
4. Pick points that are unique to each graph/differential equation. Find $\frac{dy}{dx}$ for that point and eliminate some graphs/equations. Repeat as necessary.

**Notes**

* When performing separation of variables, terms should not be added/subtracted. Only move the terms using multiplication/division. 

---
## Unit 7 Area and Volume

**Area Bounded by 2 Functions**

For areas bounded by 2 functions, there will be two intersection points. The two points where the two functions intersect are the limits of integration. 

$$
\textrm{Area between two curves}
\newline
\int_a^b  g(x) - f(x) \, dx \quad for \; g(x) \ge f(x)
$$
* The integral should always have the greater function minus the lesser function.
* If integrating to $x$, top - bottom.
* If integrating to $y$, right - left.
* The area between two functions should always be a positive number.

**Volume of Known Cross Sections**

$$
V = \int_a^b A(x) \, dx
\newline
\textrm{where A(x) is the area of the cross section}
$$

* For cross section questions, the region specified in the question is used as the base of the solid. 
* The volume is simply the sum of all the cross sections of the solid.
* Ex: If the cross section was made of semicircles, the radius is the full vertical length of the region.

**Volume of Solids of Revolution**

* Disk Method
    * Used for cases where the region is revolved around either a horizontal or vertical side of the region.
    * $V = \pi \int_a^b[r(x)]^2 \, dx$ - For revolution around a horizontal line
    * $V = \pi \int_a^b[r(y)]^2 \, dy$ - For revolution around a vertical line

* Washer Method
    * Used for cases where the revolution would have a hole
    * $V = \pi \int_a^b R(x)^2 - r(x)^2 \, dx$ - For revolution around a horizontal line
    * $V = \pi \int_a^b R(y)^2 - r(y)^2 \, dy$ - For revolution around a vertical line
    * Determine which function is $R$ and which is $r$
        * $R$ should always be the greater value and is generally the distance from the axis of revolution to the 'top' or 'right' of the region. 
        * $r$ will generally be the distance between the region and the axis of revolution.
        * Imagine the revolution and see how the region will form cylindrical cross sections. $R$ is the radius of the cylinder while $r$ is the radius of the hole. 

* Shell Method

---
## Formulas

**Differentiation/Integration**
|Differentiation|Integration|
|:---:|:---:|
$\frac{d}{dx} \, k = 0$ |
$\frac{d}{dx} \, x = 1$ | $\int \, dx = x + c$
$\frac{d}{dx} \, kf(x) = kf'(x)$ | $\int kf(x) \, dx = k \int f(x) \, dx$
$\frac{d}{dx} f(x) \pm g(x) = \frac{d}{dx}f(x) \pm \frac{d}{dx}g(x)$ | $\int f(x) \pm g(x) \, dx = \int f(x) \, dx \pm \int g(x) \, dx$
$\frac{d}{dx} f(x) g(x) = \frac{df}{dx}g(x) + \frac{dg}{dx}f(x)$ | *Integration by parts*
$\frac{d}{dx} \frac{f(x)}{g(x)} = \frac{g(x)\frac{df}{dx} - f(x)\frac{dg}{dx}}{g(x)^2}$ | 
$\frac{d}{dx} f(g(x)) = f'(g(x)) \, g'(x)$ | *See u-sub*
$\frac{d}{dx} x^n = nx^{n-1}$ | $\int x^n \, dx = \frac{x^{n+1}}{n+1} + c; n \ne -1$
$\frac{d}{dx} sin(x) = cos(x)$ | $\int sin(x) \, dx = -cos(x) + c$
$\frac{d}{dx} cos(x) = -sin(x)$ | $\int cos(x) \, dx = sin(x) + c$
$\frac{d}{dx} tan(x) = sec^2(x)$ | *Not needed*
$\frac{d}{dx} csc(x) = -csc(x)cot(x)$ | *Not needed*
$\frac{d}{dx} sec(x) = sec(x)tan(x)$ | *Not needed*
$\frac{d}{dx} cot(x) = -csc^2(x)$ | *Not needed*
$\frac{d}{dx} sin^{-1}(x) = \frac{1}{\sqrt{1-x^2}}$ |
$\frac{d}{dx} cos^{-1}(x) = -\frac{1}{\sqrt{1-x^2}}$ |
$\frac{d}{dx} tan^{-1}(x) = \frac{1}{1+x^2}$ |
$\frac{d}{dx} csc^{-1}(x) = -\frac{1}{ \|x\|\sqrt{1+x^2}}$ |
$\frac{d}{dx} sec^{-1}(x) = \frac{1}{ \|x\|\sqrt{1+x^2}}$ |
$\frac{d}{dx} cot^{-1}(x) = -\frac{1}{1+x^2}$ |
$\frac{d}{dx} e^x = e^x$ | $\int e^x = e^x + c$
$\frac{d}{dx} ln(x) = \frac{1}{x}$ | $\int \frac{1}{x} \, dx = ln\|x\| + c$
$\frac{d}{dx} a^x = ln(a) \, a^x$ | $\int a^x \, dx= \frac{a^x}{ln(a)} + c$
$\frac{d}{dx} \log_a{x} = \frac{1}{x ln a}$ | *Not needed*

**Fundamental Theorem of Calculus**

* $\int_a^b f(x) \, dx = \left.F(x)\right|_a^b = F(b) - F(a)$
* $\frac{d}{dx} \int_a^{g(x)} f(t) \, dt = f(g(x)) \, g'(x)$

**Derivative of Inverse Functions**

$$
    (f^{-1})^{'}(x) = \frac{1}{f'(f^{-1}(x))}
$$

**Average Value of $f$**

$$
\textrm{Average Value of f on} \; [a,b] = \frac{1}{b-a}\int_a^b f(x) \, dx
$$

</div>