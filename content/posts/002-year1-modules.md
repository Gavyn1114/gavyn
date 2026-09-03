+++
date = '2026-09-01'
draft = false
title = 'All UCL Maths Year 1 Modules Ranked'
slug = "first-year"
+++
I've just completed my first year at UCL studying Mathematics, and am quite pleased to be averaging a 91% :D

I thought it'd be nice to reflect a bit on the modules, so I'll be going through each module one by one, and putting them into a tier, and hopefully giving some useful advice to those studying these modules.

This post is intended for anyone interested in pursuing undergraduate mathematics (at UCL or otherwise) or anyone with a university-level mathematics background, and I've hopefully made the language accessible enough to those without a Mathematics background.

### MATH0005 Algebra 1
#### Module content
This course is an introduction to linear algebra, extending the basic matrix and vector concepts introduced in A-Level. The module begins with the basics of matrix arithmetic (multiplication, inversion, transposition) before introducing the row reduced echelon form (RREF), which is a nice way to solve large systems of linear equations, and determine if a system has a unique solution, infinitely many, or none at all.

Then, the module looks into vector spaces \(\mathbb{R}^n\) and \(\mathbb{C}^n\), where a bunch of fundamental mathematical vocabulary is introduced: linear independence, spanning sequences, bases, dimension etc. With all that machinery developed, the "most important theorem introduced in first year" can be proven: the Rank-Nullity Theorem, which informally, is a "conservation of dimension" law for matrices.

From there, we learn that matrices can also be interpreted as "linear maps", actions that stretch or rotate space. This leads into the chapter where we want to find "eigenvalues" and "eigenvectors" of  matrix. Eigenvectors are the special arrows that stay in that direction when we apply the matrix transformation, only stretched by a specific scale factor -- the eigenvalue. This is useful in the process of "diagonalising" a matrix, which is helpful for computing large powers of matrices easily with a closed-form formula.

The final chapter defines lengths and angles in multi-dimensional spaces. We use the Gram-Schmidt procedure to construct perpendicular "orthonormal" bases, and then prove the Spectral Theorem for symmetric matrices.

#### My thoughts on this module
Personally, I found this module to be really challenging the first couple weeks and was quite lost. But by exam season, I actually found myself to be very confident in this module for two reasons. One - the exam actually was extremely computational (more on this later). Two - I gradually got used to the abstraction encountered in university Mathematics throughout first year.

The exam largely focused on computing things, where you can already secure most marks by learning the essential algorithms for each chapter (solve a system of linear equations via RREF, find a basis for the kernel/column space of a matrix, apply Gram-Schmidt, compute determinants, diagonalise a matrix). I guess this made it easy to score a high number of marks, but it also made the exam really boring where it was just applying the row-reduction algorithm like five times in an exam. So I guess I wish the exam was more proof-based.

It seemed like there was a large burden of proofs initially, but it turned out that we did not need to learn 90% of the proofs to the theorems we learned in lectures, which I appreciated to a certain extent.

Overall B tier. I thought it was a nice, standard intro to linear algebra.


### MATH0003 Analysis 1
This module is really the bread and butter of university mathematics, serving as an introduction to one of the most fundamental and well-developed fields of mathematics known as Analysis. This is easily one of my favourite year 1 modules so I'll start by saying it goes straight into S tier. In simple terms, this module deconstructs all the calculus learnt at A-Levels[^1] and puts it on a rigorous foundation.

Here is a rough breakdown of the five main chapters of the course.

Chapter 1: Real numbers. This chapter introduces a lot of basic tools and definitions that will be used later on in the course and beyond - triangle inequality, the notion of boundedness, and the binomial theorem.

Chapter 2: Sequences. This chapter is concerned with the study of infinite sequences. Consider the sequence defined by \(x_n = 1/2^n\). Looking at the first few terms of the sequence, we have 1/2, 1/4, 1/8, 1/16, ... well, clearly, this sequence is "converging" towards zero, but what does that even mean? This motivates the formal definition of convergence, which is perhaps the most important definition in all of Analysis:

<div style="border-left: 4px solid #6ba3de; background: #eef4fc; padding: 1rem 1.25rem; margin: 1.5rem 0; border-radius: 4px;">
<strong>Definition (Convergence)</strong><br>
A sequence \(x_n\) converges to a limit \(L \in \mathbb{R}\) if for every \(\varepsilon > 0\), there exists \(N \in \mathbb{N}\) such that for all \(n > N\), \(|x_n - L| < \varepsilon\).
</div>


Chapter 3: Infinite series. It turns out, up to certain restrictions, it actually makes sense to sum an infinite sequence of values. For example,  the sum of 1/2, 1/4, 1/8, 1/16, ... is "clearly" one. For a general infinite series, if it has a sum, we say the infinite series converges.

Chapter 4: Limits of functions and continuity. If you were to explain what a continuous function means to a six-year-old, you'd tell them that it is a graph you can draw without lifting your hand off the paper. To formalise this very intuitive notion, you need the \(\varepsilon\text{-}\delta\) definition of continuity. The chapter culminates with a proof of the intermediate value theorem.

FIGURE: Intermediate value theorem.

Chapter 5: Differentiation. This chapter formalises what a derivative means, and proves several related theorems like the linear approximation theorem, Rolle's theorem, and the Mean Value Theorem.

I really enjoyed solving the problem sets for this module. The definitions and theorems often feel quite mysterious at first glance, but through some deep thought during problem solving, you really see why these definitions and theorems make sense and get some intuitive pictures of what they mean. Ultimately, I felt quite a deep appreciation for the mechanics of maths, seeing so many big ideas developed from such unassuming axioms.

I don't think my enjoyment of this module is shared by the majority though. Apparently, a couple hundred people scored less than 50% on the Jan midsessional exams (which are essentially mock exams). Many find the learning curve for this module in particular to be EXTREMELY steep, due to the proof-based nature of Analysis that is unlike anything seen at high school.

Advice for those taking this module:
- Learn the definitions and theorems precisely, including all the regularity assumptions (i.e. the assumptions that just ensure your mathematical object is "well behaved" enough). For example, for Rolle's Theorem or the Mean Value Theorem, you should always state that the function \(f\) is continuous on \([a, b]\) and differentiable on \((a, b)\).
- Think deeply about the subtleties - what breaks if you drop a certain assumption?  Continuing with the Rolle's Theorem/Mean Value Theorem example: why do we have to assume that \(f\) is continuous on \([a, b]\) AND differentiable on \((a, b)\) when another result in the module says that differentiability implies continuity?
- Learn all the tools at your disposal and a general idea of when you should apply them. For example, when proving that an infinite series converges, there are seven different tests you can apply. You should have several examples of series you can apply these tests to.
- Collect a zoo of counterexamples. When you learn a new theorem, it is incredibly helpful to know examples of functions or sequences where the theorem fails because one condition isn't met. For example, a classic example of a continuous function that is not differentiable on \(\mathbb{R}\) is \(f(x) = |x|\).
- Be prepared for anything. The lecturer has set fairly, routine easy exams in the past but decided to step up the difficulty significantly in May 2026, and set a paper that I thought genuinely tested deep understanding.

### MATH0004 Analysis 2
This module is a natural followup to Analysis 1, with the objective to develop a rigourous theory of integration, and then some. Again, I think this is another fantastic module, so I am putting this straight into S tier.

A rough breakdown what the module covers:

1. Cauchy sequences and uniform continuity. On its own, not a very interesting chapter, and is intended just as a warmup. However, Cauchy sequences in particular, sequences that get "really close" to each other as they progress, turn out to be very important in further mathematics. Formally:
<div style="border-left: 4px solid #6ba3de; background: #eef4fc; padding: 1rem 1.25rem; margin: 1.5rem 0; border-radius: 4px;">
<strong>Definition (Cauchy sequence)</strong><br>
A sequence \(x_n\) is Cauchy if for every \(\varepsilon > 0\), there exists \(N \in \mathbb{N}\) such that for all \(m, n > N\), \(|x_m - x_n| < \varepsilon\).
</div>

2. Riemann Integration. From the ground up, instead of loosely understanding integration as "area under the curve", the Riemann integral is formally defined using Upper and Lower Darboux sums. We see a proof of the Fundamental Theorem of Calculus, a theorem used a ton at high school without much justification for why it works.

FIGURE: FTC

Proofs are also given for other fundamental tools like integration by parts and integration by substitution, which is cool.

3. Power series. We investigate the properties of infinite series of the form \(\sum_{n=0}^{\infty} a_n x^n\), where \(a_n\) are coefficients and \(x \in \mathbb{R}\) is an independent variable. The main goal of this chapter is proving that you can differentiate and integrate them term-by-term under certain conditions. Power series are seen quite a lot in maths, for example, in Maclaurin/Taylor series. One great application of the theorems proven here is analytically justifying why \(\frac{d}{dx} exp(x) = exp(x)\) and \(\frac{d}{dx} \sin(x) = \cos(x)\).

4. L'Hôpital's rule and Taylor's theorem (which is a more general version of Maclaurin's theorem). We prove these two theorems encountered at A-Level, which is neat.

FIGURE: Lhopital

5. Improper integrals. An improper integral is, loosely speaking, an integral where something "goes wrong" - either the interval of integration is infinite, or the function blows up somewhere in the interval. This chapter is about how to prove they converge. Some examples:

<div style="text-align: center;">
\(\int_1^{\infty} \frac{1}{x^2} \, dx\) &nbsp; &nbsp; &nbsp;\(\int_{-\infty}^{\infty} e^{-x^2} dx\) &nbsp; &nbsp; &nbsp;\(\int_0^{\infty} \frac{\sin x}{x} \, dx\)
</div> 

Overall, I really enjoyed this module, gaining a really deep intuition of all the things informally examined at A-level.

Advice and thoughts for those taking this module (on top of the advice given for Analysis 1):
- The heaviest module of first year. The lecturer has said this is the module with the lowest averages across all first-year modules.
- The lecturer has kindly made typed lecture notes available (unlike the Analysis 1 lecturer), which is a great refernece to check exactly what is and isn't examinable.
- The lecturer has also made all past papers since 1997 available, which is amazing. The syllabus has not changed in the last 15 or so years, and the lecturer for this module has not changed since I was born[^2] so the exam style is fairly consistent.
- In some sense, this is the easiest module to score 100% on, as 1. there is so much "bookwork" (reciting definitions, theorem statements, and proofs) on this exam and 2. there are barely any new questions, they are all recycled from prior years. Do the past papers!
- When learning the lemmas/theorems for this module, it is often the case that the proof kind of obscures the statement and is (counterintuitively) unhelpful for understanding why the lemma/theorem is true in the first place. For example, the proof for the Taylor theorem and L'Hopital (in my opinion) does not help you understand why they are true, as they rely on some gimmicky tricks. To that end...
- When learning the lemmas/theorems for this module, I found it helpful to immediately find exam questions where they can be applied, which is helpful for understanding the statement itself.
- Don't gamble on proofs. The sheer number of proofs in this module makes it tempting to skip learning a few of them (and some really took me a long time to nail down). But they are the easiest marks to get and a tragedy to lose. Some proofs in this module can be worth so many marks. For example, the proof for Cauchy's General Principle of Convergence was worth 17 marks on one particular exam.

### MATH0006 Algebra 2
#### Module content and thoughts
An introduction to abstract algebra, the study of algebraic structures, the study of symmetry. The module is really about zooming out and looking at the underlying structure of many mathematical operations and how they're really the same under a certain lens. Another fantastic module imo, S tier.

A rough breakdown:
1. Basic number theory and permutations. Primes, divisors, Euclid's algorithm, modular arithmetic. Just a warmup to the course, nothing too exciting.

2. 
Best exam performance of mine here, scored 98/100 on this one. The lecturer is a really generous exam setter, could have set a really really diffcult exam given the nature of the module.

### MATH0008 Applied Mathematics
#### Module content and thoughts
B tier. The content is reasonably interesting but not my style of maths. The lecturer is a really harsh exam setter.

### MATH0009 Newtonian Mechanics
This module is about particle dynamics, extending ideas developed in A-Level Mechanics into 3D space. Two key themes in this module: first, developing useful coordinate systems (such as intrinsic coordinates, plane polar coordinates, and cylindrical polar coordinates), and second, using vector calculus and solving differential equations.

There are quite a few interesting problems and ideas tackled in the course. Highlights include using intrinsic coordinates to model the motion of particles sliding on a wire, calculating the trajectory of meteorites, and exploring rocket propulsion by analysing systems with variable mass.

![Gravity of Earth affecting a meteorite's trajectory.](/images/gravity_affecting_meteorite.png)
Figure 1: Gravity of Earth affecting a meteorite's trajectory.

![Rocket losing mass.](/images/rocket_losing_mass.png)
Figure 2: Rocket losing mass.

However, I wasn't that big of a fan of this module, so I'll place it in B tier. I personally found that learning about the coordinate systems was kind of dull, and the problem-solving tended to rely on too many unmotivated algebraic tricks rather than physical intuition.

Advice for those taking the module:
- Think about the physical realtiy of the problems to check if your solutions make sense.
- There are a lot of formulas in this module that you want to ensure you can derive quickly.
- When in doubt, dot with the velocity vector \(\dot{r}\).


### MATH0010 Mathematical Methods 1
#### Module content and thoughts
A very scattershot module mainly serving as a review of A-level maths content, so not that interesting.
C tier.

### MATH0010 Mathematical Methods 2
#### Module content and thoughts
C tier. This module is split into two distinct halves.

The first half is introductory Python, assuming no prior programming knowledge, so a bit dull. I really enjoy computational mathematics though, so I am really looking forward to the computational modules in Y2/3 though like Computational Methods, Numerical methods, and Combinatorial Optimisation.

The second half was an introduction to vector calculus, and introduces a bunch of fundamental theorems in calculus like Green's Theorem, Stoke's Theorem and the Gauss divergence theorem. Somewhat cool but not really my taste.

[^1]: Whenever I say A-level, I mean A-level or an equivalent curriculum like the IB.
[^2]: Which was just over 18 years ago.