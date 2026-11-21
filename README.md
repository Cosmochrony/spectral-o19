This repository contains the source of the **O19** Cosmochrony paper
*Canonical Pair Observables in Weil Blocks: The Residual Amplitude Factor and a Proposed Canonical
Normalisation with Open Tests* (titled *… Structure of the Residual Amplitude Factor and
Pipeline-Independent Formulation* up to version 1.2).

**Version 1.3.** The paper no longer claims to identify which case of its classification holds, nor
to construct a pipeline-independent canonical observable. Tests P2 and P3 are posed as open problems
and are not carried out; the former Proposition 7.2 (pipeline independence) had only a proof sketch
depending on those tests and is withdrawn as a result: it is kept, with its number, as Open
Problem 7.2. The former exclusion of the fourth case "by the q = 29 counter-example of O17" is
withdrawn: within its toy model, O17's q = 29 check verifies the raw-count block-independence identity
and computes no normalised factor, so it gives no evidence of a variation.

## Question

> If the pair observable carries a residual amplitude factor $r(c,q)$, does it come from the
> initial basis, from the block instance, or from both, and how could the pair observable be made
> canonical?

## Status of $r(c,q)$

Three statements are kept apart:

- the integer values $r(c,q)\in\{1,2,3,4\}$ are a historical hypothesis (O16 version 1.0) whose
  source is not reproduced;
- **O16** shows that on the real O12/O13 pipeline its exact conjugate-block identity forces
  $r(c,q)\equiv1$; this holds within O16's contract, not for every observable or normalisation;
- **O17** shows, within its own toy model only, that any variation of $r$ would reside entirely in
  the normalisation $D$.

## What the paper establishes

- the implicit pipeline normalisation $D(c,b_1,b_2,n)$ made explicit (Definition 2.2; the existence
  of the limit defining $r$ is assumed) and the phase invariance of the residual Gram–Schmidt increment
  (Lemma 2.1);
- a constant multiplicative factor leaves the capacity exponent $\delta_{\mathrm{pair}}$ unchanged
  (Proposition 9.1).

Lemma 2.4 (seed dependence of the rank) and Corollary 2.5 are kept unchanged but are not re-audited
in this version.

## What the paper proposes, without establishing it

- two independence tests, P2 (basis change at fixed block instance) and P3 (block-instance change at
  fixed basis), posed as Open Problems 4.1 and 5.1;
- a classification of their possible outcomes (Case A: basis artefact; Case B: instance invariant;
  Case C: mixed, $r=r_{\mathrm{base}}\,r_{\mathrm{inst}}$); a fourth case, $r$ an invariant of $(c,q)$
  alone, including $r\equiv1$, is not excluded; on O16's contract the conjugate ratio of the exact
  block observable is $1$, but that it coincides with the ratio defined here is not established;
- for each case, the construction of a canonical pair observable
  $\sigma_{\mathrm{pair}}^{\mathrm{can}}(n)$ that would follow (Definition 7.1);
- its pipeline independence, now Open Problem 7.2.

## Open problems

- the outcome of Tests P2 and P3, hence which case holds;
- the pipeline independence of the proposed canonical observable;
- whether a non-trivial $r$ occurs for any normalisation of interest, and the origin of the reported
  values;
- the stability of the proposed normalisation as $q\to\infty$ and beyond $\mathrm{Heis}_3$.

## Position in the sequence

- **O16**: pair observable introduced; on the real pipeline $r\equiv1$ within its contract
- **O17**: raw pair dynamics and the normalisation statement, both within its toy model
- **O18**: Born–Infeld parity established as a covariance of the response family; the fibre
  identification stated as an open problem
- **O19**: proposed canonical normalisation, with open tests
- **O20**, **O21**: refer to the proposed observable, not to a constructed one

# Repository Structure

```text
paper/
├── out/      # Compiled O19 PDF
├── tex/      # LaTeX sources
└── README.md
```
# Citation

If you reference this work, please cite:

J. Beau,
Canonical Pair Observables in Weil Blocks: The Residual Amplitude Factor
and a Proposed Canonical Normalisation with Open Tests,
Zenodo, 2026.

# Acknowledgements

Portions of the derivations, conceptual synthesis, numerical strategy,
and editorial refinement benefited from iterative interactions with
large language models used as analytical assistants.
All theoretical results, computations, and interpretations remain the
sole responsibility of the author.

# Contributions

This repository is intended as a research reference.

Critical feedback, independent verification, and further analysis of:

- canonical pair observables
- Gram–Schmidt-induced normalisation structure
- Weil-level amplitude classification

are welcome.

Please open an issue to discuss conceptual points,
technical details, or possible extensions.
