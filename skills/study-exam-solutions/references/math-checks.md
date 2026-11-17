# Mathematical and exam-writing checks

Read sections relevant to the problem. Independent calculations detect errors; delivered solutions still need mathematical reasoning.

## Accepting the mathematical passage in each StepBox

Hide **Why this step** and intuition-only graphics. From established data/results, a marker must be able to follow the applicable assumptions, correct formula, sufficient substitution/transformation, and conditional result. Then read the boxes consecutively for each subpart and the whole argument. A box cannot consist only of an idea, instruction to the learner, or answer table.

An intuitive graphic or finitely many numerical trials is not a general proof. Include the needed parameter branches, difference quotient, two approaching sequences, or labeled row operations. A diagram required by the problem remains part of the actual mathematical answer with construction and justification.

## Remove redundancy without removing reasoning

Each passage should add a condition, calculation, inference, answer, or learning value. Merge repetitions. A constant sequence's value and limit can share one line. Do not restate all established conditions at every conclusion. Add continuity checks, alternate methods, or printed verification only when requested or a purposeful extension; still verify internally as appropriate.

Preserve correctness-critical elements: division/cancellation conditions, exceptional branches, domains/objects, applicable theorems, decisive transformations, and a conclusion matching the scope.

## Calculus

- **Domain:** check logarithms, roots, denominators, and compositions before transformations. Preserve original exclusions after simplification.
- **Limits:** state the form, neighborhood conditions, and transformation chain. With asymptotic equivalents, check cancellation under addition/subtraction. Do not default to L'Hopital when a definition is required or the theorem is outside the course scope.
- **Epsilon–delta:** use correct quantifiers, choose delta from epsilon, and prove that choice implies the target inequality. Include denominator bounds and neighborhood conditions in the exam-ready work.
- **Piecewise continuity/differentiability:** inspect the joining value and one-sided limits. Use the difference quotient at the join when needed; derivatives of outer branches alone do not establish the derivative there.
- **Chain rule:** identify composition and rule, include every necessary derivative factor, and simplify with conditions. Each subpart needs its own application.
- **Implicit differentiation:** identify y as a function of x, differentiate every term including product-rule terms, collect y-prime, and state nonzero-denominator conditions. Analyze a zero coefficient of y-prime separately as required.
- **Integrals:** verify conditions, substitutions/bounds, and integration constants for antiderivatives. Establish improper convergence through limits before reporting a value. Differentiate to check antiderivatives.
- **Higher derivatives/formula proofs:** verify the starting index and complete the inductive step if using induction. A few examples do not establish every n.
- **Applications:** define quantities/units, model/objective, feasible domain, boundaries, and meaning of the result. Label approximations from tables/graphs with method and precision rather than presenting them as exact.

## Linear algebra

- **Matrix operations:** verify dimensions and order. For a multiplication technique being taught, show the row-column formula and enough work to determine the entries, not only a result matrix.
- **Gauss/Gauss–Jordan:** correct augmented matrix, meaningful intermediate matrices, and labeled row-operation arrows. Specify whether simultaneous additions use pre-operation or updated rows.
- **Parameters:** separate values making a pivot/denominator zero **before division**. Solve each branch, state solution count and representation, and verify consistency by substitution.
- **Inverse:** show `[A | I]` becoming `[I | A^{-1}]` with Gauss–Jordan; give a valid reason if impossible. Check by multiplying with A.
- **Determinants:** if Laplace is required, identify the chosen row/column, signs, minors, and calculations. Track row swaps, row scaling, and determinant-preserving row additions.
- **Cramer:** establish nonzero determinant before dividing. Determinant zero alone does not establish no solutions; use rank/elimination to distinguish inconsistency and infinitely many solutions.
- **Independence, span, bases, maps:** form the system in the correct orientation, analyze pivots/free variables, and interpret the result as the requested object. Distinguish dependence coefficients from vector coordinates.
- **Matrix proofs:** preserve multiplication order, square/invertibility conditions, and hypotheses. A numerical example is not a general proof; a counterexample must satisfy the stated assumptions.

## Ambiguous or missing data

Inspect the original page first. If a figure, value, or symbol is still missing, identify the exact subpart/detail and solve independent remaining parts. Label conditional results as assumptions and exclude them from verified completion counts.

## Independent verification

Choose relevant checks: substitution in the original problem, differentiating an antiderivative, multiplying a claimed inverse, a different exact rational calculation, or actually executed CAS. For parameters, check both generic and exceptional branches. Resolve contradictions before delivery.
