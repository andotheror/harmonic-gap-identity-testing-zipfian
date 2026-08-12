# Closing the Harmonic Gap: Exact Identity Testing for Zipfian Distributions

## Abstract

Instance-optimal identity testing asks how many samples are needed to test an unknown discrete distribution against a specific known null. Existing characterizations truncate a constant multiple of the testing radius. This is usually harmless, but it creates a polynomial gap for the harmonic null $q_i\propto1/i$, the canonical obstruction highlighted in a 2024 COLT open problem. We give a constant-factor characterization for the full Zipfian class $q_i\asymp1/(Li)$. Let $m_q(\varepsilon)$ be the last index whose strict suffix has null mass at least $\varepsilon$. Throughout the nondegenerate range, 

$$N^\star(q,\varepsilon) =\Theta\\!\left(L\sqrt{m_q(\varepsilon)} \max\\{1,(\varepsilon L)^{-2}\\}\right),$$

 where constants depend only on the fixed Zipf envelope. For the exact harmonic law, $L=H_k$ and $m_q(\varepsilon)=\Theta(k\exp(-\varepsilon H_k))$, so 

$$N^\star(q,\varepsilon) =\Theta\\!\left(H_k\sqrt{k e^{-\varepsilon H_k}} \max\\{1,(\varepsilon H_k)^{-2}\\}\right).$$

 Thus, for every fixed $\varepsilon\in(0,1/3]$, the answer is $\Theta((\log k)k^{(1-\varepsilon)/2})$. The upper bound combines a coarsened instance-optimal test with one unweighted tail-collision statistic. Its key step is a water-filling inequality: if almost all of a Zipfian tail is deleted, its squared discrepancy cannot fall below the tail's collision mass. The lower bound introduces a graded-thinning prior. Tail coordinate $i$ is retained with probability proportional to $i^{-1/3}$ and inflated when retained. This profile makes the alternatives $\varepsilon$-far while keeping the mixture second moment bounded up to the matching sample size. Beyond settling the harmonic example robustly, the result isolates graded thinning as the mechanism missed by constant-radius truncations.

## Contributions

- We give a constant-factor sample complexity for every fixed Zipf
envelope $q_i\asymp1/(Li)$. The exact harmonic law is a corollary with
universal constants. The answer transitions at $\varepsilon\asymp1/L$ from
the classical quadratic-accuracy rate to an accuracy-dependent effective
support.
- We introduce a two-part tester. A standard identity test is applied to
a coarsening that preserves a head and lumps the tail. If it accepts, any far
alternative must internally redistribute almost all of the tail. One
unweighted collision statistic detects exactly this case.
- We construct a matching graded-thinning prior and analyze it directly
in the fixed-sample multinomial experiment. Conditioning a single reservoir
coordinate on a typical fluctuation enforces exact normalization without
destroying the product second moment.
- We prove quantitative water-filling and thinning lemmas that expose a
common cube-root profile on the algorithmic and information-theoretic sides.

## Keywords

identity testing, distribution testing, Zipf distributions, instance optimality, sample complexity, exact constants

## Files

- `main.pdf`
- `main.tex`
- `references.bib`
- `iclr2027_conference.sty`, `iclr2027_conference.bst`, `natbib.sty`, `fancyhdr.sty`
- `main.pdf.ots`, `README.md.ots` OpenTimestamps priority proofs
