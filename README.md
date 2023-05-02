Download Link: https://assignmentchef.com/product/solved-comp350-numerical-computing-assignment-4-solving-a-nonlinear-equation
<br>
<ol>

 <li>(4 points) In class, we showed that if Newton’s iteration converges to <em>r</em>, a root of <em>f</em>(<em>x</em>) = 0, then usually it has quadratic convergence, i.e., lim<em>n</em><sub>→∞ </sub>|<em>x</em><em>n</em><sub>+1 </sub>− <em>r</em>|<em>/</em>|<em>x</em><em>n </em>− <em>r</em>|<sup>2 </sup>= <em>c</em>, where <em>c </em>= 06 is a constant. From a numerical experiment on <em>f</em>(<em>x</em>) = <em>x</em><sup>2 </sup>− 2, we found after |<em>f</em>(<em>x</em><em>n</em>)| is small enough, |<em>f</em>(<em>x</em><em>n</em>)| is squared every step. In fact it is usually true for a general nonlinear equation. Suppose <em>f</em>, <em>f</em><sup>′ </sup>and <em>f</em><sup>′′ </sup>are continuous. Prove that if <em>x</em><em>n </em>converges to a root, <em>f</em>(<em>x</em><em>n</em>) <strong>usually </strong>converges to 0 with quadratic convergence, i.e.,</li>

</ol>

lim |<em>f</em>(<em>x</em><em>n</em><sub>+1</sub>)|<em>/</em>|<em>f</em>(<em>x</em><em>n</em>)|<sup>2 </sup>= <em>c</em>

<em>n</em>→∞

for a nonzero constant <em>c</em>.

Note: Use the Taylor series theory in your analysis. The proof is not difficult.

<ol start="2">

 <li>(6 points) In class, we derived Newton’s method by using the first two terms in the Taylor series. Derive a new method by using the first three terms in the Taylor series in a similar way.</li>

</ol>

(Bonus 5 points) Show usually the new method has cubic convergence.

<ol start="3">

 <li>(10 points) Write a Matlab program m for the secant method. Suppose we want to find the largest positive root of <em>f</em>(<em>x</em>) = <em>x</em><sup>3 </sup>− 5<em>x </em>+ 3. Plot the graph of <em>y </em>= <em>f</em>(<em>x</em>) on an appropriate interval by Matlab (check how to use Matlab build-in function plot). Use your secant.m to compute the root. Also use the bisection method, the Newton method, and the new method you derived in question 2 to find the root. For the bisection method, use [1<em>,</em>3] as the initial interval, for the Newton method, use <em>x</em><sub>0 </sub>= 2 as the initial point, for the secant method, use <em>x</em><sub>0 </sub>= 1 and <em>x</em><sub>1 </sub>= 2 as the two initial points, and for the new method, use <em>x</em><sub>0 </sub>= 2 as the initial point. You can choose any appropriate initial points and initial interval, Take tolerances xtol=1.e-12 and ftol=1.e-12 for Newton’s method, the new method, and the secant method, and take delta=1.e-12 for the bisection method. Set a big number for the maximum number of iterations of the secant method and Newton’s method such that the iteration stops only when xtol=1.e-12 or ftol=1.e-12 is satisfied. Comment on the speeds of convergence of these four methods. Print out the graph of <em>y </em>= <em>f</em>(<em>x</em>) and the commands you used to plot the graph, your program secant.m, and other M-files related to <em>f</em>(<em>x</em>). Also print out the results of each iteration step. You can use M-files newton.m and bisection.m on the course web site.</li>

</ol>