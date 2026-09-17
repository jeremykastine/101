# MATH 101 Final Exam Specifications

## Purpose

This is the standing specification for generating MATH 101 (College Algebra) final exams. A future request such as "create a new MATH 101 final" or "create ten versions" should use this document unless the user explicitly changes a rule.

## Global structure

- The final contains exactly **10 main questions**, one from each problem type below.
- The exam is worth **100 points total**; each main question is worth **10 points**.
- A question may have multiple parts, but all parts should stay on that question's main topic.
- The **presentation order may be randomized by default**. The numbered problem types below are content categories, not a required presentation order.
- If a future request specifies an order, that instruction overrides randomization.
- Students may use a **basic four-function calculator only**. Scientific, graphing, CAS, and calculator-app functions are not intended to be used.
- Problems should favor exact answers and clean arithmetic. Do not require logarithm approximations or calculator features beyond four-function arithmetic.

## Version identifiers

- Do not use generic labels such as `Version A`, `Version B`, etc.
- A normally generated single exam version should use a **12-digit timestamp identifier** in the format `YYYYMMDDHHMM`, using the user's local date and time and a 24-hour clock. The timestamp is encoded to the nearest minute and contains **no punctuation**.
- Example: September 17, 2026 at 4:22 PM becomes `202609171622`.
- Display this identifier wherever the version identifier appears, including the exam booklet, student answer sheet, answer key, and combined-PDF labeling/filename when practical.
- If multiple exam versions are generated together from the same request, use the same 12-digit base timestamp and append sequential suffixes `.1`, `.2`, `.3`, and so on. Example: `202609171622.1`, `202609171622.2`, `202609171622.3`.
- The base timestamp itself remains punctuation-free; the decimal-style suffix is used only to distinguish multiple versions generated as one batch.

## Difficulty balancing across randomized versions

Randomization will cause small natural differences in item difficulty. Balance difficulty at the **whole-exam level**.

- Keep every item within the approved range for its problem type.
- If one selected item is on the harder end for its type, balance the version with one or more items on the easier end of their approved ranges.
- If several selected items are simultaneously near the upper end, revise the version rather than allowing the whole test to become substantially harder.
- Consider both conceptual difficulty and expected algebraic workload.
- Avoid accidental arithmetic complexity and extreme outliers.

## Scoring, exam booklet, answer sheet, and key

### Scoring

- Each main question is worth exactly 10 points.
- Every version must have a complete subpart scoring plan whose subparts sum to 10 points for each main question.
- Prefer whole-number point values; half-points are acceptable when appropriate (for example, four matches worth 2.5 points each).
- Point weights should reflect reasoning/work, not merely the number of blanks.

### Exam booklet

- **Do not print point values in the exam booklet by default.** Do not place `10 points`, `[2 pts]`, or similar annotations beside questions or parts unless explicitly requested later.
- Keep the exam booklet compact and readable. The answer sheet is the canonical place for detailed part labels and scoring.
- Do not vertically list a sequence of one- or two-word requested features merely because each has a separate answer-sheet row. Prefer concise prose such as: `Give the domain, range, x-intercept, y-intercept, and end behavior.`
- Keep vertical subparts when the parts represent meaningfully different procedures or a deliberate sequence of work, such as Rational Root Theorem -> candidate testing -> long division -> quadratic formula.
- Multiple-choice choices may remain vertical when clearer.
- Condense repeated wording and unnecessary whitespace without removing useful scratch-work space or making directions ambiguous.

### Student answer sheet

Every exam version must include a version-specific student answer sheet.

- Do not repeat problem statements.
- Include the version identifier, student-name area, question numbers, concise part labels, point values, and appropriately sized answer lines/boxes.
- Follow the actual randomized presentation order and numbering of that exam version.
- Each main question must visibly total 10 points. For a question with multiple parts, each part must show its own point value and the parts must sum to 10.
- **Do not create a redundant subpart for a single-part question.** If the entire question has only one response worth 10 points, show the question once with `10 points`; do not place a second `10 points` label beneath it or invent an `A`, `1`, or other part label solely for scoring.
- Concise labels such as `Domain`, `Range`, `Vertical asymptote`, `Choice`, `Graph I`, and `Solutions` are appropriate.
- For multipart rows labeled `A`, `B`, `C`, etc., `1`, `2`, `3`, etc., or similar part markers, the writing line should run essentially the **full usable width of the row**: begin immediately after the left-side part label/descriptor and continue all the way to just before the right-aligned point value. Do not leave a short isolated blank near the middle of the row.
- The same full-width-line rule applies between successive part labels and between different point values so that it is visually obvious which line belongs to which part.
- Keep the left part labels aligned in a narrow column and the point values aligned in a narrow right column, with the answer line filling the space between them.
- Use **solid horizontal separator lines only between main questions**.
- Use **dashed horizontal separator lines only between successive parts within the same main question** so part boundaries are visually distinct from question boundaries.
- A dashed part separator belongs **between** parts, not after them: a two-part question has one dashed separator, a three-part question has two, a four-part question has three, and so on.
- Do **not** draw a dashed separator below the final part of a multipart question; the solid separator for the next main question already provides the lower boundary.
- For a single-part question, do **not** draw any internal dashed separator at all; use only the main-question boundary structure.
- Avoid stacked or duplicate horizontal rules. There should never be both a dashed internal-part rule and a solid main-question rule immediately beneath the same final response area.

### Paired answer key

Every exam version must also include a paired answer key.

- Build the **answer key first as the canonical layout template**.
- The key contains expected final answers in the same answer locations as the student sheet.
- It is primarily a grading/reference sheet, not a worked-solutions document unless worked solutions are separately requested.
- Equivalent acceptable forms may be noted briefly if they fit without changing the layout.

### Exact answer-sheet/key layout matching

The student answer sheet and answer key must come from the **same layout source/template**.

- Their page count, page breaks, question placement, line lengths, row heights, spacing, left-side part labels, full-width answer lines, and right-side point-value alignment must match.
- Preferred method: typeset the complete answer key and create the student version from the same source with answer text hidden while preserving dimensions. White answer text is acceptable.
- Do not independently recreate the blank answer sheet after designing the key.
- Visually verify page-for-page alignment before delivery.
- When multiple exam versions are generated, each version receives its own matching answer sheet/key and clear version identifier.

### Combined deliverable and duplex-safe printing

By default, deliver each exam version as **one combined PDF**, not as three separate PDFs. The combined PDF must contain these three sections in this order:

1. **Exam booklet**
2. **Student answer sheet**
3. **Answer key**

The PDF must be laid out for ordinary two-sided/duplex printing so that no section begins on the back side of the final sheet of the preceding section.

- Each of the three sections must begin on an **odd-numbered PDF page**, i.e. the front side of a fresh physical sheet when printed duplex starting with page 1 as a front side.
- If the exam booklet has an odd number of pages, insert a completely blank padding page after it so the student answer sheet begins on a new sheet.
- The student answer sheet should occupy **exactly one physical sheet, front and back (2 PDF pages)**. Keep its layout compact enough to preserve this two-page requirement.
- The answer key should likewise occupy **exactly one physical sheet, front and back (2 PDF pages)** and must remain geometrically identical to the answer sheet as specified above.
- Because the answer sheet and key are each two pages, the answer key will naturally begin on a new front side when the answer sheet begins on a front side. If any future layout change would alter this, add blank padding as needed so the key still begins on an odd-numbered page.
- Padding pages must be truly blank or unobtrusively marked as intentionally blank; they must not contain exam, answer-sheet, or answer-key content.
- When multiple versions are generated, create one duplex-safe combined PDF per version unless the user explicitly requests a different packaging format.

---

# Required Problem Types

## Problem Type 1 - Composition of Functions
**Textbook:** 3.4

Multiple-choice recognition problem. Give a function `h(x)` naturally viewed as a composition and several proposed pairs `f`, `g`; the student chooses the pair satisfying `h(x)=f(g(x))`.

The skill is recognizing the inside and outside functions, not merely carrying out a specified composition. Good examples include `h(x)=sqrt(3x+7)` or `h(x)=(2x-5)^4`. Distractors may reverse inside/outside functions, misplace coefficients/constants, or confuse `f o g` with `g o f`.

## Problem Type 2 - Transformations of Functions from Graphs
**Textbook:** 3.5

Show two graphs on the same coordinate plane: original `y=f(x)` and transformed `y=g(x)`. Do not give an algebraic formula for the original. Ask the student to choose the correct function-notation relationship between `g` and `f`.

Approved transformation families:

1. translations: horizontal, vertical, or both;
2. vertical transformations: stretch/compression, x-axis reflection, or both;
3. horizontal transformations: stretch/compression, y-axis reflection, or both.

Do not combine vertical and horizontal transformation families in the same item. Do not combine scaling/reflection with translations unless this specification is later changed. Use an asymmetric/distinctive graph so the relationship is visually unambiguous.

## Problem Type 3 - Constructing a Polynomial from Its Graph
**Textbook:** 5.3

Give the graph of a degree 3, 4, or 5 polynomial. The student writes its algebraic definition, preferably in factored form.

The graph must show all real zeros clearly, make multiplicities visually identifiable by crossing/touching behavior, and include one additional labeled point to determine the leading constant `a`.

Expected reasoning: read zeros -> infer multiplicities -> write `a` times the corresponding factors -> use the additional point to solve for `a`. Choose zeros and the extra point so `a` is an integer or simple fraction.

## Problem Type 4 - Finding All Zeros of a Polynomial
**Textbook:** 5.5

Give a third- or fourth-degree polynomial with exactly two real irrational roots and either one rational root (degree 3) or two rational roots (degree 4).

Students must:

1. list **all possible rational zeros** using the Rational Root Theorem;
2. test only a small subset explicitly supplied by the problem;
3. identify the actual rational zero(s);
4. use **polynomial long division** to reduce to a quadratic;
5. use the **quadratic formula** to obtain the final two irrational roots.

The remaining quadratic must have a positive nonsquare discriminant. Do not use complex final roots. The candidate-testing subset prevents repetitive substitution while still requiring the full Rational Root Theorem candidate list.

## Problem Type 5 - Behavior of Rational Functions
**Textbook:** 5.6

Choose one of two comparable forms.

### Form A - factored, non-slant

- Numerator and denominator are already completely factored.
- No slant asymptote; use horizontal/other non-slant end behavior.
- A hole may be included and is useful.
- Typical requested features: domain, hole, vertical asymptote(s), horizontal asymptote/end behavior, x-intercept(s), y-intercept.

### Form B - simple unfactored with slant asymptote

- No hole.
- Degree 2 numerator and degree 1 denominator.
- Simple coefficients.
- Student uses polynomial division to find the slant asymptote.
- Typical requested features: domain, vertical asymptote, slant asymptote, intercepts, end behavior.

Do not make Form B simultaneously hard to factor or hide a hole. Its extra burden should mainly be polynomial division.

## Problem Type 6 - Radical Function Analysis
**Textbook:** 5.7, radical-function portion

Give a transformed square-root function algebraically. Ask for the **domain, range, x-intercept, y-intercept (when one exists), and end behavior**. In the exam booklet these may be requested compactly in one sentence; the answer sheet contains the separate labeled rows and points.

Choose parameters so endpoints/intercepts are clean and exactly computable. Reflections and shifts are allowed.

## Problem Type 7 - Matching Exponential Functions to Graphs
**Textbook:** 6.2

Show four exponential curves on the **same coordinate plane** and give four algebraic functions to match to them. Use basic functions of the form `f(x)=a b^x` with no horizontal or vertical shifts.

Students should distinguish effects such as `a` determining the y-intercept, `b>1` versus `0<b<1`, and different growth/decay rates. Prefer positive `a` unless changed later.

### Graph-style rule

- Draw **all four curves with the same solid-line style**. Do not distinguish them by dashed, dotted, dash-dotted, color-dependent, or other differing line styles.
- Identify curves by labeling them **A, B, C, and D at both the far left and the far right edges of the graphing window**, adjacent to their respective curves. Each curve therefore carries the same letter at both edges.
- Choose the functions and graphing window so the A-D edge labels are clearly separated and unambiguously associated with the curves.
- Do not make the matching solvable merely by separating growth from decay; students should need to distinguish both `a` and `b`.

## Problem Type 8 - Analysis of a Transformed Logarithmic Function
**Textbook:** 6.4

Give a transformed logarithmic function algebraically. Ask for features such as **domain, range, vertical asymptote, x-intercept, and end behavior**. In the exam booklet these may be requested in one compact sentence.

Choose base/shifts so the x-intercept is exact and reduces to a familiar power of the base. Do not require decimal log approximations. This problem is about logarithmic function behavior, not logarithm-property manipulation.

## Problem Type 9 - Logarithmic Properties and Exact Evaluation
**Textbook:** 6.5

Give one or more short exact-evaluation items using logarithmic properties. The application of the properties must make a **real difference**: avoid items whose individual logarithms are already easy to evaluate by inspection.

Approved properties: product, quotient, power, change of base. Individual subproblems should normally require only one or two properties.

Preferred common-log decimal patterns include expressions like:

- `log(0.2)+log(50)` -> `log(10)`;
- `log(7.5)-log(0.075)` -> `log(100)`;
- `2log(0.5)+log(400)` -> `log(100)`.

A change-of-base item must remain exact and hand-solvable, e.g. `log_4(8)=log(8)/log(4)=3/2`. Do not provide tables of log values and do not require numerical logarithm approximations.

## Problem Type 10 - Equation or Nonlinear-System Solving

This is the catch-all solving problem. For a randomly generated version, select the category with equal probability:

- **25% radical equation**
- **25% exponential equation**
- **25% logarithmic equation**
- **25% nonlinear system**

If the selected category has subtypes, choose among them with equal probability.

### 10A - Radical equation
**Textbook:** 5.7

Always use exactly **one radical**. Never use two-radical equations.

Two equally likely subtypes:

1. **Extraneous-solution subtype:** one radical is isolated/easy to isolate; squaring gives a factorable quadratic with two candidates; exactly one is extraneous and must be rejected by checking the original equation. Example structure: `sqrt(2x+3)=x`.
2. **Both-valid subtype:** one radical; squaring gives a quadratic; both solutions satisfy the original. Example structure: `sqrt(7x-3)=x+1`.

### 10B - Exponential equation
**Textbook:** 6.6

Use different-looking bases that can be rewritten using a common base. No logarithms or scientific calculator should be needed. Preferred structure: `8^(x-1)=4^(x+1)`, then rewrite to a common base and equate exponents.

### 10C - Logarithmic equation
**Textbook:** 6.6

The equation should be relatively straightforward but require **one logarithmic property** before conversion to exponential form.

Three equally likely subtypes:

1. product property leading to a linear equation, e.g. `log_5(x-1)+log_5(5)=2`;
2. quotient property leading to a linear equation, e.g. `log_3(x+6)-log_3(x)=1`;
3. product property leading to a quadratic plus domain rejection, e.g. `log_2(x)+log_2(x-2)=3`.

No scientific-calculator approximation.

### 10D - Nonlinear system
**Textbook:** 7.3

Two equally likely subtypes:

1. **line + parabola**, solved algebraically by substitution/equivalent method, normally producing two intersections; the resulting quadratic may factor or require the quadratic formula;
2. **line + circle**, solved by substitution, with a manageable quadratic and normally two intersections.

Exclude systems producing unnecessary quartics, systems where one variable is simply given as a constant (too trivial), and ordinary linear systems. Linear equations/systems are prerequisite material rather than a final-exam focus.

---

# Coverage philosophy

The final intentionally emphasizes function-centered College Algebra content rather than sampling every textbook section equally. Quadratic equations and ordinary linear systems do not receive dedicated questions because they are treated as prerequisite material, though quadratic solving may appear as a supporting skill in polynomial zeros, radical equations, or nonlinear systems. Domain/range are embedded naturally in function-analysis questions rather than receiving a separate problem.

Primary coverage: composition; transformations; polynomial graphs and zeros; rational functions; radical functions; exponential graphs; logarithmic functions; logarithm properties; and one randomized equation/system-solving item.

# Generation checklist

Before finalizing any version, verify:

1. exactly 10 required problem types, one each;
2. order randomized unless explicitly fixed;
3. Problem Type 10 obeys 25/25/25/25 category probability when randomness is requested;
4. Problem Type 10 subtypes are equally likely within their category;
5. exam is solvable with at most a four-function calculator;
6. no item accidentally requires scientific/graphing/CAS features;
7. graphs are legible and intended features are unambiguous;
8. exponential matching uses four same-style solid curves with A-D labels at both left and right edges;
9. multiple-choice distractors are plausible and clearly incorrect;
10. exact values are used wherever possible;
11. Rational Root Theorem item requires all candidates but provides a limited subset to test;
12. polynomial-zero item uses long division and ends in a quadratic with two real irrational roots;
13. rational-function item conforms to approved Form A or Form B;
14. radical/logarithmic function-analysis prompts use clean exact features;
15. logarithm-property items genuinely benefit from the properties;
16. whole-exam difficulty/workload is balanced across randomized selections;
17. each main question is worth 10 points, total 100;
18. exam booklet omits point annotations by default;
19. short feature lists are condensed in the exam booklet when appropriate;
20. answer sheet/key show the complete subpart scoring plan;
21. version-specific answer sheet and key are generated from the same layout template;
22. answer sheet contains no problem statements;
23. key and answer sheet have matching page count, page breaks, spacing, and answer-line geometry;
24. exam, answer sheet, and key share the same version identifier;
25. final delivery is one combined PDF in the order exam -> answer sheet -> answer key;
26. each section begins on an odd-numbered PDF page/front side of a fresh duplex sheet;
27. blank padding pages are inserted wherever needed to prevent one section from printing on the back of another;
28. answer sheet is exactly 2 pages and answer key is exactly 2 pages;
29. version identifier uses `YYYYMMDDHHMM` rather than a lettered version label;
30. if multiple versions are generated in one batch, they use the same timestamp plus `.1`, `.2`, `.3`, etc. suffixes.
31. answer-sheet/key separators use solid rules between main questions and dashed rules only between internal parts;
32. no dashed separator appears after the final part or in a single-part question, and no duplicate/stacked horizontal rules remain.
33. multipart answer-sheet/key rows use full-width response lines from the part label to just before the right-aligned point value;
34. single-part 10-point questions are not redundantly broken into a one-item subpart with a second 10-point label.
