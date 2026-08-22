+++
date = '2026-06-28'
draft = false
title = 'All UCL Maths Year 1 Modules Ranked'
slug = "first-year"
+++
DRAFT.
I've just completed my first year at UCL studying Mathematics, and am quite pleased to be averaging a 91% :D

I thought it'd be nice to reflect a bit on the modules, so I'll be going through each module one by one, and putting them into a tier.

This post is intended for anyone interested in pursuing undergraduate mathematics, perhaps at UCL, or anyone with a university-level mathematics background.

### MATH0005 Algebra 1
#### Module content
This course is an introduction to linear algebra, extending the basic matrix and vector concepts introduced in A-Level (or equivalent). The module begins with the basics of matrix arithmetic (multiplication, inversion, transposition) before introducing the row reduced echelon form (RREF), which is a nice way to solve large systems of linear equations, and determine if a system has a unique solution, infinitely many, or none at all.

Then, the module looks into vector spaces \(\mathbb{R}^n\) and \(\mathbb{C}^n\), where a bunch of fundamental mathematical vocabulary is introduced: linear independence, spanning sequences, bases, dimension etc. With all that machinery developed, the "most important theorem introduced in first year" can be proven: the Rank-Nullity Theorem, which informally, is a "conservation of dimension" law for matrices.

From there, we learn that matrices can also be interpreted as "linear maps", actions that stretch or rotate space. This leads into the chapter where we want to find "eigenvalues" and "eigenvectors" of  matrix. Eigenvectors are the special arrows that stay in that direction when we apply the matrix transformation, only stretched by a specific scale factor -- the eigenvalue. This is useful in the process of "diagonalising" a matrix, which is helpful for computing large powers of matrices easily with a closed-form formula.

The final chapter defines lengths and angles in multi-dimensional spaces. We use the Gram-Schmidt procedure to construct perpendicular "orthonormal" bases, and then prove the Spectral Theorem for symmetric matrices.

#### My thoughts on this module
Personally, I found this module to be really challenging the first couple weeks and was quite lost. But by exam season, I actually found myself to be very confident in this module for two reasons. One - the exam actually was extremely computational (more on this later). Two - I gradually got used to the abstraction encountered in university Mathematics throughout first year.

The exam largely focused on computing things, where you can already secure most marks by learning the essential algorithms for each chapter (solve a system of linear equations via RREF, find a basis for the kernel/column space of a matrix, apply Gram-Schmidt, compute determinants, diagonalise a matrix). I guess this made it easy to score a high number of marks, but it also made the exam really boring where it was just applying the row-reduction algorithm like five times in an exam. So I guess I wish the exam was more proof-based.

It seemed like there was a large burden of proofs initially, but it turned out that we did not need to learn 90% of the proofs to the theorems we learned in lectures, which I appreciated to a certain extent.

Overall B tier. I thought it was a nice, standard intro to linear algebra.


### MATH0003 Analysis 1
#### Module content and thoughts
This module is really the bread and butter of university mathematics, serving as an introduction to one of the most fundamental and well-developed field of mathematics known as Analysis. Easily one of my favourite year 1 modules so I'll start by saying it goes straight into S tier.

The module starts with only the basic properties of real numbers and provides rigorous proofs for some main results in elementary calculus. This module is divided into four chapters.

Chapter 1: Real numbers. This chapter introduces a lot of basic tools and definitions that will be used later on in the course - triangle inequality, the notion of boundedness, supremum, infimum, maximum, minimum, and the binomial theorem.

Chapter 2: Sequences. One big thing analysts are concerned about is taming infinity. This chapter is concerned with the study of infinite sequences. Consider the sequence defined by \(x_n = 1/2^n\). Looking at the first few terms of the sequence, we have 1/2, 1/4, 1/8, 1/16, ... Well clearly, this sequence is "converging" towards zero, but how can we prove it? This motivates the formal definition of convergence:

A sequence \(x_n\) converges to a limit \(L\) in \(\mathbb{R}\) if for every \(\varepsilon > 0\), there exists \(N\) in \(\mathbb{N}\) such that for all \(n \geq N\), \(|x_n - L| < \varepsilon\).

which is perhaps the most important definition in all of Analysis.

Also in this chapter: algebra of limits for sequences, sandwich theorem (aka squeeze theorem, two policemen theorem, ...), divergence, monotone convergence theorem.

write stuff on subsequences? Which turns out to be a really important idea (Bolzano-Weistrass)


### MATH0004 Analysis 2
#### Module content and thoughts
A natural followup to Analysis 1, with the objective to develop a rigourous theory of integration.

S tier, fantastic module.

### MATH0006 Algebra 2
#### Module content and thoughts
S tier again. An introduction to abstract algebra. Really cool seeing how through abstraction, many mathematical operations are structually the "same" in some sense.

Best exam performance of mine here, scored 98/100 on this one. The lecturer is a really generous exam setter, could have set a really really diffcult exam given the nature of the module.

### MATH0008 Applied Mathematics
#### Module content and thoughts
B tier. The content is reasonably interesting but not my style of maths. The lecturer is a really harsh exam setter.

### MATH0009 Newtonian Mechanics
#### Module content and thoughts
C tier. Again, not really my style of maths. This module is kind of like A-level mechanics but in 3D, so lots and lots of vectors. Some pretty interesting stuff though, like the study of orbital motion, and studying the motion of objects on a surface of revolution.

### MATH0010 Mathematical Methods 1
#### Module content and thoughts
A very scattershot module mainly serving as a review of A-level maths content, so not that interesting.
C tier.

### MATH0010 Mathematical Methods 2
#### Module content and thoughts
C tier. This module is split into two distinct halves.

The first half is introductory Python, assuming no prior programming knowledge, so a bit dull. I really enjoy computational mathematics though, so I am really looking forward to the computational modules in Y2/3 though like Computational Methods, Numerical methods, and Combinatorial Optimisation.

The second half was an introduction to vector calculus, and introduces a bunch of fundamental theorems in calculus like Green's Theorem, Stoke's Theorem and the Gauss divergence theorem. Somewhat cool but not really my taste.