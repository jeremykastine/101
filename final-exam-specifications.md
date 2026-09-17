# MATH 101 Final Exam Specifications

## Purpose

This document is the standing specification for generating new versions of the MATH 101 (College Algebra) final exam. A future request such as "create one new version of the MATH 101 final" or "create ten different versions" should be carried out from this document unless the user explicitly changes a rule.

## Global structure

- The final contains **10 required problem types**.
- Each generated exam contains exactly one problem from each required type.
- Each main question is worth **10 points**, for **100 points total**.
- A main question may have multiple parts, but all parts should remain focused on that question's primary topic.
- The presentation order may be **randomized by default**. The numbering of the problem types below identifies content categories, not a required presentation order.
- If a future request specifies an order, that instruction overrides the default randomization rule.
- Questions should emphasize conceptual understanding, algebraic structure, and exact hand-solvable work rather than calculator-dependent approximation.

### Calculator policy

- Students may use a **basic four-function calculator**.
- Scientific calculators, graphing calculators, CAS calculators, calculator apps, and similar tools are not intended to be used.
- Construct problems so required logarithms, exponents, radicals, roots, intercepts, and other values are exact or obtainable with simple arithmetic.
- A four-function calculator may reduce arithmetic burden but should not replace the mathematical skill being assessed.

### Difficulty balancing across randomized versions

Randomization will naturally create some variation in difficulty. Versions should be balanced by **overall exam difficulty and workload**, not by forcing every instance of every problem type to be mechanically identical.

- If one selected problem is on the harder end of its approved type, balance the version with one or more problems on the easier end of their approved ranges.
- If several randomly selected problems are simultaneously near the upper end of their difficulty ranges, revise the version rather than allowing the whole exam to become substantially harder than another version.
- Avoid extreme outliers even if they technically satisfy the topic specification.
- Consider both conceptual difficulty and expected algebraic work.

### General construction principles

- Prefer clean integers, simple fractions, and exact radicals.
- Avoid accidental arithmetic complexity.
- Graphs must make intended features visually clear and should not rely on tiny visual distinctions.
- Multiple-choice distractors should represent plausible misconceptions rather than arbitrary wrong answers.
- When a problem is intended to assess a particular method, choose numbers so that method is genuinely useful.
- Unless approximation is explicitly being tested, answers should be exact.

## Scoring and point allocation

- Every main question is worth exactly **10 points**.
- Every generated exam must explicitly show the point value of each labeled subpart.
- Subpart values within each main question must total exactly 10 points.
- A question with no meaningful subparts may be treated as one 10-point part.
- When a question naturally contains independently gradable components, make those components explicit subparts whenever practical.
- Prefer whole-number point values when practical. Half-point values are acceptable when they produce a cleaner division, such as four equally weighted matches worth 2.5 points each.
- Point weights should reflect expected reasoning and work, not merely the number of blanks.
- The exam, student answer sheet, and answer key must show the same point allocations.

## Student answer sheet and paired answer key

Every generated final-exam version must have a **version-specific student answer sheet** and a **paired answer key** in addition to the exam itself.

### Student answer sheet

- Do **not** repeat the problem statements.
- Include only the version identifier, student-name area, question numbers, concise part labels, point values, and appropriately sized answer lines or boxes.
- Follow the actual presentation order and numbering of that exam version.
- Each main question must visibly total 10 points, and each subpart must show its point value.
- Concise labels such as `Domain`, `Range`, `Vertical asymptote`, `Choice`, `Graph I`, or `Solutions` are appropriate.
- Give enough room for the expected final answer, but do not duplicate the exam booklet's scratch-work space.

### Answer key

- Build the **answer key first as the canonical layout template** for the answer sheet.
- Put the expected final answer in each answer location.
- Use the same question numbers, labels, point values, line lengths, spacing, page breaks, and overall geometry as the student sheet.
- The key is primarily a grading/reference sheet, not a full worked-solutions document, unless worked solutions are separately requested.
- If several mathematically equivalent answer forms should be accepted, the key may note an equivalent form if it fits without changing the layout.

### Exact layout matching requirement

The student answer sheet and answer key must come from the **same layout source/template**.

- Preferred method: typeset the complete key, then generate the student sheet from the same source with the answer text hidden while preserving exact dimensions.
- White answer text on the student version is acceptable when it preserves line wrapping, row heights, and page breaks exactly.
- Do not independently recreate the student sheet after designing the key.
- The answer sheet and key must have the same page count, matching page breaks, matching question placement, and matching vertical/horizontal spacing.
- Visually verify the pair page-for-page before delivery.
- When multiple exam versions are created, each version must receive its own matching answer sheet and key, with the same clear version identifier on all three artifacts.

---

# Required Problem Types

## Problem Type 1 - Composition of Functions

**Textbook section:** 3.4 - Composition of Functions

### Format

A **multiple-choice recognition problem**.

- Give a function `h(x)` naturally viewed as a composition of two simpler functions.
- Give several choices, each proposing `f` and `g` such that the choice claims `h(x)=f(g(x))`.
- The student selects the correct decomposition.

### Intended skill

Recognize the inside and outside functions rather than merely compute a composition already specified.

### Approved examples

- `h(x)=sqrt(3x+7)` with correct decomposition `f(x)=sqrt(x)`, `g(x)=3x+7`.
- `h(x)=(2x-5)^4` with correct decomposition `f(x)=x^4`, `g(x)=2x-5`.

### Distractors

Useful distractors include reversing inside/outside functions, moving coefficients or constants outside the wrong operation, applying only part of the expression, or confusing `f o g` with `g o f`.

---

## Problem Type 2 - Transformations of Functions from Graphs

**Textbook section:** 3.5 - Transformation of Functions

### Format

A **graph-interpretation multiple-choice problem**.

- Show two graphs on the same coordinate plane.
- Label one `y=f(x)` and the other `y=g(x)`.
- Do not give an algebraic definition for the original graph.
- Ask which function-notation relationship correctly describes `g` in terms of `f`.

### Approved transformation families

Use one family per generated item:

1. **Translations:** horizontal shift, vertical shift, or both together.
2. **Vertical transformations:** vertical stretch/compression, x-axis reflection, or both.
3. **Horizontal transformations:** horizontal stretch/compression, y-axis reflection, or both.

Do not combine vertical and horizontal transformation families in the same item. Do not combine scale/reflection families with translations unless this specification is changed later.

Use an asymmetric or distinctive graph so the transformation is unambiguous.

---

## Problem Type 3 - Constructing a Polynomial from Its Graph

**Textbook section:** 5.3 - Graphs of Polynomial Functions

### Format

Give the graph of a polynomial of degree **3, 4, or 5**. The student writes an algebraic definition, preferably in factored form.

The graph must show:

- all real zeros clearly;
- multiplicities through crossing versus touching/turning behavior;
- one additional labeled point that determines the leading constant.

### Required reasoning

The student should identify zeros, infer multiplicities, write a factored form with leading constant `a`, use the labeled point to determine `a`, and state the final polynomial.

Choose the extra point so `a` is an integer or simple fraction whenever possible.

---

## Problem Type 4 - Finding All Zeros of a Polynomial

**Textbook section:** 5.5 - Zeros of Polynomial Functions

### Format

Give a third- or fourth-degree polynomial with exactly two real irrational roots and either:

- one rational root for degree 3; or
- two rational roots for degree 4.

### Required methods

The student must:

1. use the **Rational Root Theorem** to list all possible rational zeros;
2. test a small specified subset of those candidates;
3. identify the actual rational zero(s);
4. use **polynomial long division** to reduce to a quadratic;
5. use the **quadratic formula** to find the final two irrational roots.

The student must list all possible rational zeros, but the problem itself should specify which small subset to test so the task does not become repetitive substitution.

The final quadratic must have a positive nonsquare discriminant, giving two real irrational roots. Do not use complex final roots here.

---

## Problem Type 5 - Behavior of Rational Functions

**Textbook section:** 5.6 - Rational Functions

Use one of two approved forms of comparable overall difficulty.

### Form A - Factored, no slant asymptote

- Numerator and denominator are already completely factored.
- End behavior uses a horizontal asymptote or another non-slant case.
- A removable discontinuity/hole may be included.
- Typical requested features: domain, hole, vertical asymptote, horizontal asymptote/end behavior, x-intercepts, and y-intercept.

The algebra is easy to read; the difficulty is structural interpretation.

### Form B - Simple unfactored with a slant asymptote

- No hole.
- Degree 2 numerator.
- Degree 1 denominator.
- Simple coefficients.
- The student uses polynomial division to find the slant asymptote.
- Typical requested features: domain, vertical asymptote, slant asymptote, intercepts, and end behavior.

Do not combine difficult factoring or a hidden hole with the slant-asymptote version.

---

## Problem Type 6 - Radical Function Analysis

**Textbook section:** 5.7 - Inverses and Radical Functions, radical-function portion

### Format

Give a transformed square-root function algebraically. Ask for:

- domain;
- range;
- x-intercept;
- y-intercept when one exists;
- end behavior.

Choose parameters so intercepts and endpoint behavior are exact and clean. Reflections and shifts are allowed.

---

## Problem Type 7 - Matching Exponential Functions to Graphs

**Textbook section:** 6.2 - Graphs of Exponential Functions

### Format

- Show four exponential graphs on one coordinate plane.
- Give four exponential functions algebraically.
- Students match each function to its graph.

Use basic functions of the form `f(x)=a*b^x` with no horizontal or vertical shifts.

The set should require students to distinguish several of the following:

- `a` determines the y-intercept;
- `b>1` gives growth;
- `0<b<1` gives decay;
- larger versus smaller bases change growth/decay rate.

Prefer positive `a` unless changed later. Do not make the item solvable merely by separating growth from decay; include shared y-intercepts and/or shared general behavior.

---

## Problem Type 8 - Analysis of a Transformed Logarithmic Function

**Textbook section:** 6.4 - Graphs of Logarithmic Functions

### Format

Give a transformed logarithmic function algebraically and ask for features such as:

- domain;
- range;
- vertical asymptote;
- x-intercept;
- end behavior.

Choose the base and shifts so the x-intercept is exact and reduces to a familiar power of the base. Do not require decimal logarithm approximations. This problem is about logarithmic-function structure and behavior, not logarithm-property manipulation.

---

## Problem Type 9 - Logarithmic Properties and Exact Evaluation

**Textbook section:** 6.5 - Logarithmic Properties

### Purpose

Using logarithm properties should make a **real difference**. Avoid expressions where each individual logarithm is already easy to evaluate by inspection.

### Format

The student evaluates one or more logarithmic expressions exactly without a scientific calculator.

- Do not provide a table of logarithm values.
- Use common logarithms and/or carefully chosen bases.
- Each short subproblem should normally require only one or two logarithmic properties.

Approved properties:

- product property;
- quotient property;
- power property;
- change-of-base formula.

### Preferred decimal style

Use decimal arguments that individually are inconvenient but combine to powers of 10, for example:

- `log(0.2)+log(50)=log(10)`;
- `log(7.5)-log(0.075)=log(100)`;
- `2log(0.5)+log(400)=log(100)`.

### Change-of-base style

Change of base should remain exact and hand-solvable. Example:

`log_4(8)=log(8)/log(4)=3log(2)/(2log(2))=3/2`.

Do not require decimal logarithm approximation.

---

## Problem Type 10 - Equation or Nonlinear-System Solving

This is the catch-all **solving** problem. The other nine types focus primarily on functions and function behavior.

### Top-level randomization

For a random version, choose with equal probability:

- **25% Radical equation**
- **25% Exponential equation**
- **25% Logarithmic equation**
- **25% Nonlinear system**

When a selected category has approved subtypes, select those subtypes with equal probability as well.

### 10A - Radical equation

**Textbook section:** 5.7

Always use **one radical only**. Do not use two-radical equations.

Two equally likely subtypes:

#### Radical subtype A - easier, one extraneous solution

- The radical is isolated or very easy to isolate.
- Squaring leads to a factorable quadratic with two algebraic candidates.
- Exactly one candidate is extraneous and must be rejected by checking the original equation.

Example: `sqrt(2x+3)=x`.

#### Radical subtype B - somewhat more challenging, both valid

- Still one radical.
- Squaring leads to a quadratic.
- Both resulting solutions satisfy the original equation.

Example: `sqrt(7x-3)=x+1`.

### 10B - Exponential equation

**Textbook section:** 6.6

Use an exponential equation with different-looking bases that can be rewritten with a common base. No logarithms or scientific calculator should be needed.

Preferred structure: `8^(x-1)=4^(x+1)`.

The intended method is to rewrite both sides using the same base and equate exponents.

### 10C - Logarithmic equation

**Textbook section:** 6.6

Require **one logarithmic property** before converting to exponential form and solving.

Three equally likely subtypes:

1. Product property leading to a linear equation, e.g. `log_5(x-1)+log_5(5)=2`.
2. Quotient property leading to a linear equation, e.g. `log_3(x+6)-log_3(x)=1`.
3. Product property leading to a quadratic with one solution rejected by the logarithmic domain, e.g. `log_2(x)+log_2(x-2)=3`.

No scientific-calculator approximation should be required.

### 10D - Nonlinear system

**Textbook section:** 7.3 - Systems of Nonlinear Equations and Inequalities: Two Variables

Two equally likely approved subtypes:

#### Nonlinear subtype A - line and parabola

- Solve by substitution or equivalent algebraic method.
- Resulting quadratic must be manageable by hand.
- Normally produce two intersection points.
- The quadratic may factor or require the quadratic formula if overall workload remains appropriate.

Example:

`y=x^2`, `y=x+2`.

#### Nonlinear subtype B - line and circle

- Solve by substitution.
- Resulting quadratic must be manageable by hand.
- Normally produce two intersection points.

Example:

`x^2+y^2=25`, `y=x+1`.

### Exclusions for nonlinear systems

- No unnecessarily complicated quartics after substitution.
- No trivial case where one variable is simply given as a constant, such as a circle with `y=2`.
- No ordinary linear systems; linear equations and linear systems are prerequisite material rather than a focus of this final.

---

# Coverage philosophy

This final intentionally emphasizes function-centered College Algebra content rather than sampling every textbook section equally.

- No dedicated quadratic-equation question is required. Quadratic solving may appear as a supporting skill inside polynomial zeros, radical equations, or nonlinear systems.
- Domain and range do not require a stand-alone problem because they appear naturally in radical, logarithmic, rational, and other function-analysis questions.

The final concentrates on composition, transformations, polynomial graph structure and zeros, rational-function behavior, radical functions, exponential and logarithmic functions, logarithm properties, and one randomized solving problem.

# Generation checklist

Before finalizing any version, verify:

1. Exactly 10 required problem types are present, one of each.
2. Presentation order is randomized unless a fixed order was requested.
3. Problem Type 10 follows the 25/25/25/25 top-level selection rule when random generation is requested.
4. Problem Type 10 subtypes are equally likely within their selected category.
5. The exam is solvable with at most a four-function calculator.
6. No item accidentally requires a scientific or graphing calculator.
7. Graphs are legible and intended features are visually unambiguous.
8. Multiple-choice distractors are plausible but clearly incorrect.
9. Exact values are used wherever possible.
10. Rational-root problems require the full Rational Root Theorem candidate list but provide a limited set of candidates to test.
11. Polynomial-zero problems use polynomial long division and end in a quadratic with two real irrational roots.
12. Rational-function problems conform to approved Form A or Form B.
13. Radical- and logarithmic-function analysis problems use clean intercepts and exact behavior.
14. Logarithm-property problems genuinely benefit from applying logarithm properties.
15. Overall difficulty and expected work are reviewed and balanced across randomized selections.
16. No excluded structure has slipped into Problem Type 10.
17. Each main question is worth exactly 10 points, for 100 points total.
18. Every labeled subpart displays a point value and each main question sums to 10 points.
19. A version-specific student answer sheet and paired answer key are generated.
20. The student answer sheet contains no problem statements, only numbering, concise labels, point values, and answer spaces.
21. The answer key and student sheet come from the same layout source and have matching page count, page breaks, spacing, and answer-line geometry.
22. The exam, answer sheet, and key carry the same clear version identifier and matching point allocations.
