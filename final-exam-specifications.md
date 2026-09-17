# MATH 101 Final Exam Specifications

## Purpose of this document

This document is the standing specification for generating new versions of the MATH 101 (College Algebra) final exam. It is intended to be detailed enough that a future request such as "create one new version of the MATH 101 final" or "create ten different versions of the final" can be carried out without redefining the exam structure.

Unless this document is explicitly revised, future versions should follow these specifications.

---

## Global exam structure

- The final contains **10 problem types**.
- A problem may contain multiple parts, but all parts of that problem should stay focused on the same main topic or skill.
- Each generated exam should contain **exactly one problem from each of the 10 problem types** described below.
- The **presentation order may be randomized by default**. The labels "Problem Type 1" through "Problem Type 10" in this document identify the required content categories, not necessarily the order in which they must appear on a generated exam.
- If a future request explicitly specifies an order, that instruction overrides the default randomization rule.
- Questions should emphasize conceptual understanding, algebraic structure, and hand-solvable exact work rather than calculator-dependent numerical approximation.

### Calculator policy

- Students may use a **basic four-function calculator**.
- Scientific calculators, graphing calculators, CAS calculators, calculator apps, and similar tools are not intended to be used.
- Problems should therefore be designed so that all required logarithms, exponents, radicals, roots, intercepts, and other values can be obtained exactly or with simple arithmetic.
- A four-function calculator may reduce arithmetic burden, but it should not replace the mathematical skill being assessed.

### Difficulty balancing across randomized versions

Randomization will inevitably create some natural variation in difficulty. Generated versions should be checked as a whole for comparable workload and difficulty.

- Do not try to force every instance of every problem type to be mechanically identical in difficulty.
- Instead, aim for a comparable **overall exam difficulty**.
- If one randomly generated item appears to be on the harder end of its approved problem type, balance the version by making one or more other items fall on the easier end of their approved ranges.
- Likewise, if several randomly selected items are simultaneously near the upper end of their difficulty ranges, revise the version rather than allowing the whole exam to become substantially harder than another version.
- Avoid extreme outliers even if they technically satisfy a topic specification.
- Difficulty balancing should consider both conceptual difficulty and expected amount of algebraic work.

### General construction principles

- Prefer clean integer, fractional, or exact radical answers.
- Avoid accidental arithmetic complexity.
- Graphs must make all intended features visually clear and should not rely on tiny visual distinctions.
- Distractors in multiple-choice questions should be plausible and should correspond to recognizable misconceptions rather than arbitrary wrong answers.
- When a problem is intended to assess a particular method, construct the numbers so that the method is genuinely useful and not merely decorative.
- Unless a problem specifically tests approximation, answers should be expressible exactly.

---

# Required Problem Types

## Problem Type 1 - Composition of Functions

**Textbook section:** 3.4 - Composition of Functions

### Format

This is a **multiple-choice recognition problem**.

- Give a function `h(x)` that is naturally viewed as a composition of two simpler functions.
- Give several answer choices, each proposing functions `f` and `g` such that the choice claims `h(x)=f(g(x))`.
- The student selects the pair whose composition actually reproduces the given function.

### Intended skill

The student should recognize the **inside function** and the **outside function**, rather than merely compute a composition that has already been specified.

### Approved style examples

- `h(x)=sqrt(3x+7)`, with the correct decomposition `f(x)=sqrt(x)`, `g(x)=3x+7`.
- `h(x)=(2x-5)^4`, with the correct decomposition `f(x)=x^4`, `g(x)=2x-5`.

### Distractor guidance

Useful distractors include reversing the inside and outside functions, moving a coefficient or constant outside the wrong operation, applying only part of the original expression, or confusing `f o g` with `g o f`. The correct choice should be unambiguous after actual substitution.

---

## Problem Type 2 - Transformations of Functions from Graphs

**Textbook section:** 3.5 - Transformation of Functions

### Format

This is a **graph interpretation multiple-choice problem**.

- Show two graphs on the **same coordinate plane**.
- Clearly identify one as the original function `y=f(x)`.
- Clearly identify the other as the transformed function `y=g(x)`.
- Do **not** provide an algebraic definition for the original graph.
- Ask the student to choose the function-notation relationship that correctly describes `g` in terms of `f`.

Example answer style: `g(x)=f(x-3)+2`.

### Approved transformation families

A generated version may use one of the following families:

1. **Translations** - horizontal shift, vertical shift, or both together.
2. **Vertical transformations** - vertical stretch/compression, reflection across the x-axis, or both.
3. **Horizontal transformations** - horizontal stretch/compression, reflection across the y-axis, or both.

Do not combine the vertical-transformation family and horizontal-transformation family in the same item. Do not combine scaling/reflection families with translations unless this specification is explicitly changed later.

### Intended skill

The student should infer transformations from graphical evidence and express the relationship correctly in function notation, including the sign reversal inherent in horizontal shifts and horizontal scalings.

### Graph-design guidance

Use an asymmetric or otherwise distinctive original graph so the transformation is clear. Label the two curves directly or use a very clear legend. Avoid graphs whose symmetry makes two different transformations visually indistinguishable.

---

## Problem Type 3 - Constructing a Polynomial from Its Graph

**Textbook section:** 5.3 - Graphs of Polynomial Functions

### Format

Give the graph of a polynomial of **degree 3, 4, or 5**. The student must write an algebraic definition of the polynomial.

The graph must provide enough information to determine the polynomial uniquely up to the expected factored form:

- all real zeros are visually identifiable;
- multiplicities are identifiable from the graph's behavior at each zero;
- one additional labeled point is provided to determine the leading constant.

### Required reasoning

The student should read the zeros from the graph, infer multiplicities from whether the graph crosses or touches/turns at each zero, write `f(x)=a(x-r1)^m1(x-r2)^m2...`, substitute the additional point to solve for `a`, and give the final polynomial, preferably in factored form unless another form is requested.

### Example structure

A fourth-degree graph might have `x=-2` with multiplicity 2, `x=1` with multiplicity 1, `x=3` with multiplicity 1, and labeled point `(0,12)`. This leads to `f(x)=a(x+2)^2(x-1)(x-3)`, and the extra point determines `a`.

### Construction constraints

The zeros and multiplicities must be visually unambiguous. The additional point should produce a manageable value of `a`, preferably an integer or simple fraction. Avoid excessive vertical scale that makes the graph unreadable.

---

## Problem Type 4 - Finding All Zeros of a Polynomial

**Textbook section:** 5.5 - Zeros of Polynomial Functions

### Format

Give a **third- or fourth-degree polynomial** with exactly two real irrational roots and either one rational root (degree 3) or two rational roots (degree 4).

### Required methods

The student must:

1. use the **Rational Root Theorem** to list all possible rational zeros;
2. test a small specified subset of those candidates;
3. identify the actual rational zero or zeros;
4. use **polynomial long division** to reduce the polynomial to a quadratic;
5. use the **quadratic formula** to find the final two irrational roots.

### Candidate-testing rule

The student is responsible for listing **all possible rational zeros**, but the problem should then explicitly tell the student which small subset of those candidates to test. This prevents the problem from becoming an exercise in repetitive substitution.

### Degree-specific structure

- **Degree 3:** one rational root and two irrational roots.
- **Degree 4:** two rational roots and two irrational roots.

### Root constraints

The remaining quadratic should have a **positive, nonsquare discriminant** so that the last two roots are real and irrational. Do not use complex final roots for this problem type.

### Example approved structure

`f(x)=x^4-x^3-4x^2+2x+4`, which has rational zeros `-1` and `2` and irrational zeros `+/-sqrt(2)`. A generated problem need not use this exact polynomial, but the structure is appropriate.

---

## Problem Type 5 - Behavior of Rational Functions

**Textbook section:** 5.6 - Rational Functions

There are two approved forms. They should be treated as alternate ways to assess comparable overall skill, with one emphasizing structural interpretation and the other emphasizing algebraic processing.

### Form A - Factored rational function, no slant asymptote

- Give numerator and denominator already **completely factored**.
- End behavior should involve a horizontal asymptote or another non-slant case.
- A removable discontinuity (hole) may be included and is useful in this form.

Typical requested features may include domain, holes, vertical asymptotes, horizontal asymptote/end behavior, x-intercepts, and y-intercept.

Because the expression is already factored, the difficulty comes from correctly interpreting factors, cancellations, excluded values, and graph behavior.

### Form B - Simple unfactored rational function with a slant asymptote

- **No hole.**
- Numerator has degree 2.
- Denominator has degree 1.
- Coefficients should be simple.
- The student should use polynomial division to identify the slant asymptote.

Typical requested features may include domain, vertical asymptote, slant asymptote, intercepts, and end behavior.

### Difficulty-equivalence principle

Form B should not also contain difficult factoring or a hidden hole. Its main additional algebraic burden is polynomial division. Form A may contain more structural features because the factoring work has already been done.

---

## Problem Type 6 - Radical Function Analysis

**Textbook section:** 5.7 - Inverses and Radical Functions (radical-function portion)

### Format

Give a **transformed square-root function** algebraically. Ask the student to determine domain, range, x-intercept, y-intercept when one exists, and end behavior.

### Construction guidance

Choose parameters so intercepts and endpoints are clean and exactly computable. The problem should focus on understanding the transformed square-root function, not on difficult arithmetic. Reflections and shifts are allowed.

Example appropriate form: `f(x)=-2sqrt(x+1)+4`.

---

## Problem Type 7 - Matching Exponential Functions to Graphs

**Textbook section:** 6.2 - Graphs of Exponential Functions

### Format

- Show **four exponential graphs on the same coordinate plane**.
- Give **four exponential functions algebraically**.
- Students match each function to its graph.

### Function family

Use basic functions of the form `f(x)=a*b^x` with no horizontal or vertical shifts. Transformations are already assessed elsewhere.

### Intended distinctions

The set should require students to use several of the following ideas:

- `a` determines the y-intercept;
- `b>1` gives growth;
- `0<b<1` gives decay;
- among growth functions, different bases create different growth rates;
- among decay functions, different bases create different decay rates.

Prefer positive values of `a` unless this specification is later changed.

### Construction guidance

Do not make the task solvable merely by separating growth from decay. Include functions with shared y-intercepts and/or shared general behavior so students must distinguish both `a` and `b`.

---

## Problem Type 8 - Analysis of a Transformed Logarithmic Function

**Textbook section:** 6.4 - Graphs of Logarithmic Functions

### Format

Give a transformed logarithmic function algebraically, such as `f(x)=2+log_3(x-4)`. Ask the student to determine features such as domain, range, vertical asymptote, x-intercept, and end behavior.

### Construction guidance

Choose the base and shifts so that the x-intercept can be found exactly without a scientific calculator. The intercept should reduce to a familiar power of the base. Avoid requiring decimal logarithm approximations. This question is about the structure and behavior of logarithmic functions, not logarithm-property manipulation; logarithm properties are assessed separately in Problem Type 9.

---

## Problem Type 9 - Logarithmic Properties and Exact Evaluation

**Textbook section:** 6.5 - Logarithmic Properties

### Purpose

This problem should make the use of logarithm properties **genuinely useful**. Avoid expressions where each individual logarithm is already easy to evaluate by inspection.

### General format

The student evaluates one or more logarithmic expressions exactly, using logarithmic properties to transform them into forms that can be evaluated without a scientific calculator.

- Do not provide a table of logarithm values in advance.
- Use common logarithms and/or carefully chosen bases.
- Each individual subproblem should normally require only **one or two logarithmic properties**.
- If the question contains several short subparts, keep each one concise.

### Approved property types

- product property;
- quotient property;
- power property;
- change-of-base formula.

### Preferred decimal style

Decimal arguments are especially useful because the original logarithms may not be obvious, while the transformed expression becomes a power of 10.

Approved example structures include:

- `log(0.2)+log(50)=log(10)`;
- `log(7.5)-log(0.075)=log(100)`;
- `2log(0.5)+log(400)=log(100)`.

### Change-of-base style

A change-of-base item should still remain exact and hand-solvable. For example, `log_4(8)=log(8)/log(4)=3log(2)/(2log(2))=3/2`. The change-of-base formula may be combined with a simple power-property observation, but should not require decimal logarithm approximation.

---

## Problem Type 10 - Equation or Nonlinear-System Solving

This is the exam's **catch-all solving problem**. The other problem types focus primarily on functions and function behavior; this one focuses directly on solving an equation or nonlinear system.

### Top-level randomization

When generating a random version, choose the Problem Type 10 category with equal probability:

- **25% Radical equation**
- **25% Exponential equation**
- **25% Logarithmic equation**
- **25% Nonlinear system**

When a selected category contains approved subcategories, those subcategories are also chosen with equal probability unless this specification is explicitly changed.

### 10A - Radical equation

**Textbook section:** 5.7

Always use a **one-radical equation**. Do not use two-radical equations.

There are two equally likely approved subtypes:

#### Radical subtype A - easier equation with an extraneous solution

- One radical is isolated or very easy to isolate.
- Squaring leads to a factorable quadratic with two algebraic candidates.
- Exactly one candidate is extraneous and must be rejected by checking in the original equation.

Approved structural example: `sqrt(2x+3)=x`.

#### Radical subtype B - somewhat more challenging, both solutions valid

- Still only one radical.
- Squaring leads to a quadratic.
- Both resulting solutions satisfy the original equation.

Approved structural example: `sqrt(7x-3)=x+1`.

The difficulty difference between the two subtypes comes from algebra and checking, not from introducing a second radical.

### 10B - Exponential equation

**Textbook section:** 6.6

Use an exponential equation with **different-looking bases that can be rewritten using a common base**. The student should not need logarithms or a scientific calculator.

Preferred structure: `8^(x-1)=4^(x+1)`. The intended method is to rewrite both sides with the same base and equate exponents. Generated variants may change the bases and linear expressions in the exponents, but should preserve this basic level of difficulty and exact solvability.

### 10C - Logarithmic equation

**Textbook section:** 6.6

The equation should be relatively straightforward but require **one logarithmic property** before converting to exponential form and solving.

There are three approved subtypes, selected with equal probability when the logarithmic-equation category is chosen:

#### Log subtype A - product property leading to a linear equation

Example structure: `log_5(x-1)+log_5(5)=2`.

#### Log subtype B - quotient property leading to a linear equation

Example structure: `log_3(x+6)-log_3(x)=1`.

#### Log subtype C - product property leading to a quadratic and domain rejection

Example structure: `log_2(x)+log_2(x-2)=3`. The algebra produces two candidates, but the original logarithmic domain eliminates one.

No scientific-calculator logarithm approximation should be required.

### 10D - Nonlinear system

**Textbook section:** 7.3 - Systems of Nonlinear Equations and Inequalities: Two Variables

There are two equally likely approved subtypes:

#### Nonlinear-system subtype A - line and parabola

- Solve by substitution or an equivalent algebraic method.
- The resulting quadratic should be manageable by hand.
- The system should normally produce two intersection points.
- The quadratic may factor cleanly or may require the quadratic formula, provided the overall workload remains appropriate.

Example structure: `y=x^2` and `y=x+2`.

#### Nonlinear-system subtype B - line and circle

- Solve by substitution.
- The resulting quadratic should be manageable by hand.
- The system should normally produce two intersection points.

Example structure: `x^2+y^2=25` and `y=x+1`.

### Excluded nonlinear-system structures

- Do not use systems that produce an unnecessarily complicated quartic after substitution.
- Do not use overly trivial systems in which one variable is simply given as a constant (for example, a circle together with `y=2`).
- Do not use ordinary linear systems; linear equations and linear systems are treated as prerequisite material rather than a focus of this final.

---

# Coverage philosophy

This final intentionally emphasizes the function-centered content of College Algebra rather than attempting to give every textbook section equal representation.

The exam does **not** require a dedicated quadratic-equation question. Quadratic solving may appear as a supporting skill inside polynomial-zero problems, radical equations, or nonlinear systems, but quadratics are treated primarily as prerequisite knowledge.

Likewise, domain and range do not require a stand-alone problem because they are naturally incorporated into radical, logarithmic, rational, and other function-analysis questions.

The final therefore concentrates on composition and transformations; polynomial graph structure and zeros; rational-function behavior; radical-function behavior; exponential and logarithmic graphs/functions; logarithm properties; and one randomized equation/system-solving problem.

---

# Generation checklist

Before finalizing any generated exam version, verify all of the following:

1. There are exactly 10 required problem types, one of each.
2. Presentation order is randomized unless the user explicitly requested a fixed order.
3. Problem Type 10 follows the 25% / 25% / 25% / 25% category-selection rule when random generation is requested.
4. Any Problem Type 10 subcategory is selected with equal probability among its approved subtypes.
5. The exam is solvable with at most a four-function calculator.
6. No item accidentally requires a scientific or graphing calculator.
7. Graphs are legible and all intended features are visually unambiguous.
8. Multiple-choice distractors are plausible but clearly incorrect.
9. Exact values are used wherever possible.
10. Rational-root problems explicitly require the full Rational Root Theorem candidate list but provide a limited set of candidates to test.
11. Polynomial-zero problems use polynomial long division and end in a quadratic with two real irrational roots.
12. Rational-function problems conform to either approved Form A or Form B.
13. Radical-function and logarithmic-function analysis problems use clean intercepts and exact behavior.
14. Logarithm-property questions genuinely benefit from applying logarithm properties.
15. The total difficulty and expected work are reviewed as a whole; harder-than-average random selections are balanced by easier selections elsewhere.
16. No prohibited or intentionally excluded structures have slipped into Problem Type 10.
