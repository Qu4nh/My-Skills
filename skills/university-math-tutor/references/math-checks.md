# Mathematical checks by subject

Read only the sections relevant to the current course and exercise; do not print this checklist or introduce techniques outside onboarded theory. Actually compute and verify. Missing data prevents a verdict.

## Across subjects

- Identify the objects, domains, hypotheses, notation, units, and requested conclusion before transforming anything.
- Distinguish equivalent transformations from one-way implications. Check divisions, squaring, roots, logarithms, extraneous solutions, endpoints, and excluded parameter values against the original problem.
- A graph or finite numerical check supports intuition/error detection, not a general proof. Keep exact and approximate results distinct and state error/precision when relevant.
- Check by a genuinely appropriate alternative: substitution, differentiation, normalization, a small finite enumeration, an independently computed quantity, or actually executed exact computation.

## Single-variable calculus

- **Limits:** check punctured-neighborhood domains, one-sided limits, and valid cancellations. Simplification does not restore an excluded original point. Inspect cancellation before using asymptotic equivalents. Use L'Hopital only when taught and its hypotheses hold.
- **Definitions/proofs:** preserve epsilon–delta quantifier order and the dependence of delta on epsilon. A few approaching values are not a limit proof; to disprove a limit using sequences, exhibit valid sequences with incompatible limiting values.
- **Continuity/differentiability:** include the function value at a joining point. Derivatives of surrounding branches alone do not establish the derivative there; use the applicable difference quotient/limit argument.
- **Derivatives:** apply all chain/product/implicit factors and retain nonzero-denominator conditions. Check nondifferentiable points or singular branches instead of substituting into a formula derived away from them.
- **Integration:** verify substitutions, bounds, antiderivative constants, and hypotheses for using the fundamental theorem. Distinguish signed accumulation from geometric area. For improper integrals, establish convergence before reporting a value; differentiate to check antiderivatives.
- **Sequences/series:** distinguish convergence, absolute convergence, and divergence. Verify hypotheses of comparison/ratio/other taught tests; a failed or inconclusive test is not divergence. Check power-series endpoints separately from the interior radius.

## Multivariable calculus and analytic geometry

- Specify point, coordinate system, domain, and whether a vector represents direction, position, or displacement. Verify norms, inner products, and projection assumptions.
- For a directional derivative defined per unit distance, normalize the direction vector; distinguish it from a path derivative whose speed matters. Partial derivatives alone do not prove total differentiability.
- For extrema, check stationary points, boundary/constraint cases, and conditions of the Hessian or multiplier test. An inconclusive test is not a classification; local and global extrema differ.
- For multiple integrals or changes of variables, verify regions, transformed bounds, Jacobian absolute value where required, and relevant invertibility/interchange hypotheses. Do not infer metric facts from an unscaled sketch.

## Linear algebra

- For AB, verify dimensions and order; entry `(i,j)` uses row i of A and column j of B. Preserve intermediate matrices and label decisive row/column operations.
- For a minor \(M_{ij}\), remove the correct row/column and take the determinant. \(C_{ij}=(-1)^{i+j}M_{ij}\) differs from \(a_{ij}\). Laplace expansion fixes one row/column; include every term and sign.
- Row exchange reverses determinant sign; row scaling multiplies it by that factor; adding another row's multiple preserves it. Track mixed operations. Triangular determinants use diagonal products; block-triangular matrices need square diagonal blocks, not necessarily invertible ones.
- The cofactor matrix is \((C_{ij})\), while \(\operatorname{adj}(A)=(C_{ij})^T\). \(A^{-1}=\operatorname{adj}(A)/\det A\) requires square A and nonzero determinant; check a claimed inverse by multiplication.
- Gauss–Jordan applies row operations simultaneously to \([A\mid I]\). Arbitrary column operations do not allow reading the right block as the inverse. Separate zero pivots/parameter branches before division.
- For a singular system, inspect rank/compatibility rather than inferring no solution from determinant zero. Distinguish dependence coefficients, coordinates, spanning sets, bases, and mapping directions.
- When block methods are actually covered, verify dimensions/invertibility: for A invertible use \(D-CA^{-1}B\); for D invertible use \(A-BD^{-1}C\). Preserve order. Do not assume \(\det\begin{pmatrix}A&B\\C&D\end{pmatrix}=\det(AD-BC)\) without suitable extra hypotheses.

## Probability and introductory statistics

- Define the sample space, events/random variables, support, and model assumptions. Distinguish ordered/unordered and with/without-replacement sampling.
- \(P(A\mid B)=P(A\cap B)/P(B)\) requires \(P(B)>0\). The conditioning group changes the denominator. Do not confuse conditional probability with intersection, independence with mutual exclusion, or \(P(A\mid B)\) with \(P(B\mid A)\).
- Check probabilities lie in [0,1] and total mass/integrated density is 1 over the actual support. A density value is not a point probability for a continuous variable. Use the correct distribution, parameters, and tail.
- For expectation/variance/covariance, use correct probabilities or density, required finite moments, and independence assumptions for simplified formulas. Variance is not the expectation squared.
- Distinguish population parameters from sample statistics and variance conventions, including the relevant n versus n−1 denominator. Check estimator, sampling, independence, approximation, and degrees-of-freedom assumptions taught in the source.
- For intervals/tests, identify the target parameter, statistic/distribution, confidence/significance level, one/two-sided choice, and conclusion actually supported. Do not reinterpret a frequentist confidence interval as a posterior probability without a separate model.

## Discrete mathematics, logic, and counting

- Preserve quantifiers and domains; distinguish a statement, converse, inverse, and contrapositive. Check both directions of an equivalence when required.
- Induction needs a valid base case and the stated implication from the induction hypothesis to the next case; several verified small cases are not induction.
- Counting cases must be exhaustive and disjoint, or corrected for overlap. Check order, repetition, constraints, and double counting. Small enumeration can verify a finite case, not prove an unrestricted formula.
- For recurrences, check initial conditions and the range of indices as well as the recurrence. Graph arguments must respect directed/undirected status, loops, connectivity, and the specific theorem's hypotheses.

## Introductory differential equations and numerical methods

- Verify a proposed solution by differentiation and substitution in the original equation plus initial/boundary conditions, over its claimed domain.
- Division by an expression involving the unknown can lose equilibrium/singular solutions; inspect its zero case first. Include constants and parameter restrictions correctly. Do not assert uniqueness without applicable source hypotheses.
- Keep exact solutions separate from approximations. For a numerical method, check its input assumptions, convergence/stability conditions, step size, stopping criterion, units, and absolute/relative error as relevant.
- A small residual alone does not guarantee small solution error for an ill-conditioned problem; more iterations or a smaller step is not an unconditional accuracy guarantee. Discuss these distinctions only at the level covered by the source.

## Feedback and evidence

Separate final-answer correctness, the step causing an error, and the skill actually demonstrated. A correct number does not establish correct reasoning or broad mastery. Identify affected components after verifying the mathematics, and request the relevant intermediate work when the cause is unclear. Track the course and topic for each piece of evidence.
