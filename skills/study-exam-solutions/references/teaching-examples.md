# Transferable methods and valid shortcuts

These examples illustrate reasoning depth and purpose, not mandatory methods or fixed step counts. Put each exam-ready passage inside the corresponding learning step below its **Why this step** commentary. The continuous passages here help verify mathematics; they do not require printing a duplicate solution after the boxes.

## Example 1: rationalizing a limit

**Problem:** Find \(\lim_{x\to0}(\sqrt{1+x}-1)/x\).

**Reusable method — conjugates:** When a root difference gives 0/0, consider the conjugate. Check the root's domain and denominator, then use \((a-b)(a+b)=a^2-b^2\). Preserve the original excluded point after cancellation.

**Step 1 — Choose the transformation.** Why: multiplying by \(\sqrt{1+x}+1\) produces the needed factor x. Multiply both numerator and denominator, not only the numerator.

**Step 2 — Cancel and take the limit.** Why: x is nonzero in the punctured neighborhood, and the new denominator tends to a nonzero value.

**Exam-ready passages for the boxes:** For \(x>-1\) and \(x\ne0\),
\[
\frac{\sqrt{1+x}-1}{x}
=\frac{(\sqrt{1+x}-1)(\sqrt{1+x}+1)}{x(\sqrt{1+x}+1)}
=\frac{(1+x)-1}{x(\sqrt{1+x}+1)}
=\frac{1}{\sqrt{1+x}+1}.
\]
The square-root function is continuous at 1 and the denominator tends to 2, hence
\[
\lim_{x\to0}\frac{\sqrt{1+x}-1}{x}
=\frac{1}{\sqrt{1+0}+1}=\boxed{\frac12}.
\]

**Transfer:** For \(a>0\) and constant b, rationalization gives
\(\lim_{x\to0}(\sqrt{a+bx}-\sqrt a)/x=b/(2\sqrt a)\).
Derive it rather than memorizing an answer. The case a=0 is excluded and requires separate domain/one-sided analysis. Do not present differentiation as the standard method if it is outside the learner's course scope.

**Self-check:** Replace the numerator with \(\sqrt{4+3x}-2\). What is the limit, and why exclude x=0 before simplifying?

**Answer for the end of the document:** \(3/4\); the original expression divides by x, while the limit uses nonzero x near zero.

## Example 2: preserve a parameter branch

**Problem:** Solve \(x+y=2\), \(x+my=m+1\) for real m.

**Reusable method — eliminate, then inspect the pivot:** Subtract the first equation from the second. If the remaining coefficient depends on a parameter, inspect its zero case before dividing. Distinguish \(0=0\) from \(0=c\ne0\).

**Exam-ready passages for the boxes:**
\[
\left[\begin{array}{cc|c}1&1&2\\1&m&m+1\end{array}\right]
\xrightarrow{R_2\leftarrow R_2-R_1}
\left[\begin{array}{cc|c}1&1&2\\0&m-1&m-1\end{array}\right].
\]
If \(m\ne1\), the second equation gives \(y=(m-1)/(m-1)=1\), then \(x=2-1=1\). The solution is uniquely \((1,1)\).

If \(m=1\), the second row is \(0=0\), leaving \(x+y=2\). With \(y=t\in\mathbb R\), \(x=2-t\), so the solution set is \(\{(2-t,t):t\in\mathbb R\}\).

Internally substitute into both original equations. When the argument already uses valid equivalent transformations and no verification is requested, there is no need to print a repetitive substitution check.

**Recognition shortcut:** Equal coefficients of x suggest subtraction to expose m−1. It saves work while remaining writable in an exam. Cancelling \((m-1)/(m-1)\) for every m loses the branch m=1.

**Self-check:** Change the second right-hand side to m+2. At m=1, are there still infinitely many solutions?

**Answer for the end:** No; elimination gives \(0=1\), so the system is inconsistent.
