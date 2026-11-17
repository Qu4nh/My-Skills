# Adaptive ELI5 and mathematical visuals

## Adapt to evidence

ELI5 means **fewer hidden assumptions**, not childish language or omitted mathematics. Start with purpose and an observable operation before naming its formula. Avoid opening with a dense sequence of definitions.

| Feedback/evidence | Next adjustment |
|---|---|
| "I do not understand" / "Why that step?" | Locate the obstacle, change representation to a small numerical/labeled example, and expose the hidden step. Ask one diagnostic only if the obstacle is still unclear |
| Understands the idea but misses signs/indices | Keep intuition brief, label the relevant positions/sign, and repair locally rather than reteaching the chapter |
| Calculates correctly without explaining why | Recognize the calculation; check the decisive reason/condition when needed, without claiming broad mastery |
| Solves and explains correctly; wants speed | Focus on the new variation/condition and reduce repeated examples or elementary arithmetic |
| Understands but asks how to write an exam answer | Turn that idea into a complete mathematical passage with conditions, without duplicating the entire solution |

Do not infer preferences from an unspecified age, major, culture, or educational system. Start with small labeled examples and update from responses. Choose anchors from the actual course and demonstrated prerequisites; do not use a matrix example merely because the tutor once taught linear algebra.

## Select a visual for the obstacle

| Obstacle | Show directly | Connection to notation |
|---|---|---|
| Limit versus value at a point | A small value table or graph with the target point distinguished from nearby inputs | Approaching a point uses nearby domain values; it is not simply substituting an undefined value |
| Derivative or local rate | A labeled secant becoming a tangent, or two nearby inputs and the difference quotient | Average change approaches the instantaneous rate under the derivative's conditions |
| Integral and accumulation | Signed strips/partition table with interval and axes labeled | An integral accumulates signed contributions; area requires separate sign handling |
| Several variables | A slice/contour diagram with point and direction labeled | Specify which variable moves and normalize direction when measuring rate per unit distance |
| Conditional probability | A two-way count table or restricted sample-space diagram | Rebuild the denominator from the conditioning event |
| Statistical summary/inference | Labeled observations or sampling diagram, separating data from the target parameter | A sample statistic and a population quantity play different roles |
| Counting/induction | A small labeled choice tree, exhaustive cases, or base-case/inductive-step diagram | Count each admissible object once; a checked example differs from a general proof |
| Differential equation | A slope/direction table or field when supported; label initial point and equilibrium | Local rates constrain solution curves, and division may discard constant solutions |
| Minor versus cofactor | Removed row/column, remaining submatrix, relevant sign | The minor is its determinant; the cofactor also includes the positional sign |
| `(-1)^(i+j)` | Labeled 3-by-3 sign table | Sign depends on position, not the sign of the original entry |
| Adjugate | Cofactor matrix → transpose arrow → adjugate | Entry `(i,j)` moves to `(j,i)` |
| Matrix product | One `1×n` row and `n×1` column with the result entry labeled | Entry `(i,j)` is row i dotted with column j; order matters |
| Elimination and determinants | Before matrix → labeled row operation → after matrix | State its determinant effect at the operation |
| Parameter/possibly zero pivot | Two branches: pivot nonzero and pivot zero | Division belongs only to the nonzero branch |
| Schur complement | A 2-by-2 block matrix and elimination below the pivot block | Preserve block dimensions and multiplication order |
| Geometric determinant intuition | Labeled parallelogram/coordinates and oriented area when useful | Geometry supplies intuition; properties supply the proof |

## Example: a calculus limit (original illustration, not a source problem)

When rationalization is covered by the course, explain why a root difference suggests a conjugate. For
\[
\lim_{x\to0}\frac{\sqrt{1+x}-1}{x},
\]
the original expression is undefined at 0, but the limit concerns nearby nonzero x. In a sufficiently small neighborhood with x>−1 and x≠0,
\[
\frac{\sqrt{1+x}-1}{x}
=\frac{(\sqrt{1+x}-1)(\sqrt{1+x}+1)}{x(\sqrt{1+x}+1)}
=\frac{1}{\sqrt{1+x}+1}.
\]
The new denominator tends to 2, so the limit is 1/2. A labeled arrow `root difference → conjugate → removable factor → limit` shows why the transformation helps; it does not redefine the original expression at 0. This is a worked conceptual illustration: if that limit is the learner's pending task, use different data or stop before its answer instead.

## Example: conditional probability (original illustration)

For the question "Why does the denominator change?", show a count table:

| Group | B | Not B | Total |
|---|---|---|---|
| A | 30 | 10 | 40 |
| Not A | 20 | 40 | 60 |
| Total | 50 | 50 | 100 |

"Given B" means looking only at the 50 entries in column B. Of those, 30 are in A. Thus \(P(A\mid B)=30/50=3/5\), while \(P(A\cap B)=30/100\) describes the whole group. Connect the visual to \(P(A\mid B)=P(A\cap B)/P(B)\), with \(P(B)>0\). Label the table as original, preserve the events' meanings, and use different data if these are the learner's assigned numbers in hint mode.

## Example: cofactor sign (original illustration, not a source problem)

Learner: "Why is there a minus sign at C12?"

Separate two operations: **compute the remaining determinant**, then **apply the positional sign**. The positional sign is not the sign of the entry being removed.

For a labeled original example distinct from the current assignment,
\[
B=\begin{pmatrix}2&7&1\\0&3&4\\5&6&8\end{pmatrix}.
\]
For \(C_{12}\), remove **row 1** and **column 2**. The remaining rows 2,3 and columns 1,3 give
\[
\underbrace{\begin{pmatrix}0&4\\5&8\end{pmatrix}}_{\text{remaining submatrix}}
\quad\Longrightarrow\quad M_{12}=0\cdot8-4\cdot5=-20.
\]

| Row / column | 1 | 2 | 3 |
|---|---|---|---|
| 1 | + | − | + |
| 2 | − | + | − |
| 3 | + | − | + |

Position (1,2) has a negative multiplier, so \(C_{12}=(-1)^{1+2}M_{12}=-(-20)=20\). An exam-ready line is
\[
C_{12}=(-1)^{1+2}\begin{vmatrix}0&4\\5&8\end{vmatrix}=20.
\]
A negative positional multiplier can produce a positive cofactor when the minor is negative.

Stay on the conceptual question. If the learner is assigned C12 in their actual problem, use only the sign pattern, a general formula, or different example data; never substitute the assigned numbers into a worked illustration. If an example accidentally matches the target, choose another or use symbols.

## Connect Schur complements to elimination

Use only when Schur complements are relevant and included in the applicable source scope, or clearly identified as a permitted extension. Introduce scalar elimination first if its prerequisite is missing. Let
\[
M=\begin{pmatrix}A&B\\C&D\end{pmatrix},\qquad
A\in\mathbb R^{p\times p},\quad D\in\mathbb R^{q\times q},\quad A\text{ invertible}.
\]
To eliminate C, subtract a multiple of the top block row from the bottom. The multiplier is \(CA^{-1}\), since \(CA^{-1}A=C\):
\[
\underbrace{\begin{pmatrix}I_p&0\\-CA^{-1}&I_q\end{pmatrix}}_{\text{block elimination, determinant }1}
\begin{pmatrix}A&B\\C&D\end{pmatrix}
=\begin{pmatrix}A&B\\0&D-CA^{-1}B\end{pmatrix}.
\]
The remaining block \(D-CA^{-1}B\) is the Schur complement of A. When computing a determinant, this gives \(\det M=\det A\det(D-CA^{-1}B)\). Do not reorder the product or apply this branch when A is singular. In hint mode, reveal only the portion needed for the current task, not the entire derivation automatically.

## Readable rendering

- One idea per paragraph; immediately explain what to notice in each figure, table, or formula.
- Use `\(...\)` inline and `\[...\]` for displayed mathematics. If the host does not render it, supply aligned labeled plain text rather than repeatedly broken LaTeX.
- In matrices, `&` separates columns and **two backslashes `\\`** separate rows. Check equal column counts, balanced groups, and closed environments before sending.
- Keep algebraic grouping explicit: parenthesize a sum or difference used as a factor. An underbrace or explanatory label does not replace the parentheses needed to make the equation unambiguous.
- Labels, signs, and arrows must work without color. Avoid unsupported extended LaTeX syntax.
- Explain an analogy's mapping and limits. Matrix blocks resemble scalars in elimination, but products do not freely commute and inverses may not exist.
- A visual supports intuition; it does not replace proof or hide a step behind "obvious."
