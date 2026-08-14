This repository contains the source of the **O19** Cosmochrony paper  
*Canonical Normalisation of Pair Observables in Weil Blocks:
Eliminating Pipeline Dependence in the Gram–Schmidt Span Tracker*.

This work extends the **spectral admissibility sub-programme** by resolving the
next structural issue left open by **O18**:

> Does the residual amplitude factor arise from the initial basis, from the block instance, or from both, and how can the corresponding pair observable be made canonical?


# Context

**O18** establishes that:

- the Born–Infeld action is even, and parity acting simultaneously on configuration and probe
  acts **covariantly** on the Born–Infeld response family (even-order responses preserved, odd-order reversed)
- evenness does **not** force fixed-probe indiscernibility of \(\chi\) and \(-\chi\);
  the identification of the parity orbit with a fibre of \(\Pi\) is an **open problem**
- in the Weil realisation, the conjugation identity \(\rho_{q-c} = \overline{\rho_c}\)
  and \(\delta_{q-c} = \delta_c\) are O17 theorems (recalled in O18 Theorem 3.1), while the
  identification of \(\{c, q-c\}\) as a physical fibre of \(\Pi\) is an open bridge
- the pair-level quantity
  \[
  \sigma_{\mathrm{pair}}(n)=\sigma_c(n)\,\sigma_{q-c}(n)
  \]
  therefore keeps the status of a **structurally motivated hypothesis**

However, a residual issue remained:

- the amplitude of the pair observable still depends on the implementation-level
  normalisation inherited from the O12/O13 Gram–Schmidt pipeline
- this dependence is encoded in a residual integer factor \(r(c,q)\)
- the exponent \(\delta_{\mathrm{pair}}\) is unaffected, but the observable is not
  yet fully intrinsic

This defines the scope of **O19**.


# Core Result

The paper makes explicit the previously implicit pipeline normalisation
\[
D(c,b_1,b_2,n)
\]
and determines the dependence structure of the residual amplitude factor
\[
r(c,q).
\]

It shows that the relevant question is not whether \(r\) affects the scaling law
it does not, but whether it is:

- a pure basis artefact
- a discrete block-instance invariant
- or a mixed quantity with both components

The paper then constructs the corresponding canonical observable
\[
\sigma_{\mathrm{pair}}^{\mathrm{can}}(n),
\]
independent of pipeline conventions.

The contribution of O19 is therefore precise:

> it does not modify the observable class or the exponent,  
> it removes the last layer of pipeline dependence at the amplitude level.


# Main Structural Results

## 1. Explicit normalisation factor

The previously implicit normalisation factor of the Gram–Schmidt span tracker is
made explicit in terms of residual Gram–Schmidt increments.

This promotes the implementation-level quantity \(D(c,b_1,b_2,n)\) to a genuine
mathematical object.

## 2. Separation of raw span and normalised observable

The paper distinguishes explicitly between:

- \(\Sigma^{(c)}(n)\), the raw cumulative span
- \(\sigma_c(n)\), the normalised observable derived from it

The factor \(r(c,q)\) originates at the level of \(\Sigma^{(c)}(n)\) and is
propagated unchanged into \(\sigma_c(n)\), whereas the asymptotic exponent
\(\delta_c\) is defined at the level of \(\sigma_c(n)\).

## 3. Phase-invariance lemma

A lemma establishes that the residual Gram–Schmidt increment is invariant under
global phase multiplication of the seed vector, and that under
\[
U \in U(q)
\]
it varies only when the relative orbit alignment changes.

Therefore:

> any variation of \(D\) under the basis test captures alignment effects only,
> not a property of the representation itself.

## 4. Dependence tests P2 and P3

Two distinct tests are introduced:

- **P2:** vary the initial basis by unitary changes of basis of \(\mathbb{C}^q\)
  while fixing the block instance
- **P3:** vary the block instance \((b_1,b_2)\) while fixing a rigid basis convention

These tests determine whether \(r\) is basis-dependent, instance-dependent, or both.

## 5. Three-way classification of the residual factor

The paper identifies three possible scenarios:

- **Case A:** \(r\) is a pure basis artefact
- **Case B:** \(r\) is a discrete instance invariant
- **Case C:** \(r\) decomposes into both components

In the mixed case, the paper introduces the factorisation
\[
r = r_{\mathrm{base}}\,r_{\mathrm{inst}}.
\]

## 6. Canonical observable construction

Depending on the case realised, the canonical pair observable is constructed by:

- choosing a canonical basis choice adapted to the central action
- quotienting by the instance invariant
- or combining both steps in the mixed case

Thus the observable becomes independent of pipeline conventions even though the
route to canonicalisation depends on the dependence structure of \(r\).


# Mathematical Role of O19

The key mathematical contribution of O19 is to convert a residual implementation
dependence into a classified structural object.

More precisely, the paper proves that:

- the asymptotic law is unchanged by the residual factor
- the residual factor can be isolated at the amplitude level
- the possible sources of this factor can be separated empirically and formally
- a corresponding canonical observable can then be defined

The central point is:

> O19 is not a paper about changing \(\delta_{\mathrm{pair}}\),  
> but about making the amplitude structure intrinsic.


# Observable Hierarchy (Refined)

With O19, the observable hierarchy becomes:

- raw span level:
  \[
  \Sigma^{(c)}(n)
  \]
- normalised block observable:
  \[
  \sigma_c(n)
  \]
- pair observable:
  \[
  \sigma_{\mathrm{pair}}(n)=\sigma_c(n)\,\sigma_{q-c}(n)
  \]
- canonical pair observable:
  \[
  \sigma_{\mathrm{pair}}^{\mathrm{can}}(n)
  \]

The key statement becomes:

> the physically relevant observable was fixed in O16–O18,  
> and O19 now fixes its canonical amplitude normalisation.


# Interpretation of the Result

The conceptual significance of O19 is that the remaining residual factor is no
longer treated as a numerical nuisance.

Instead, it is analysed as a structured remainder of the Gram–Schmidt pipeline,
possibly reflecting:

- phase alignment effects
- block-instance multiplicities
- or both

The classification is determined empirically by the P2/P3 tests.
Any phase-based or multiplicity-based interpretation follows the result of this
classification, rather than being assumed in advance.

Thus, O19 provides a clean separation between:

- observable definition
- amplitude normalisation
- asymptotic scaling


# Structural Role of O19

O19 occupies a very specific place in the O-series:

- **O16**: pair observable identified
- **O17**: pair dynamics derived
- **O18**: Born–Infeld parity established as a covariance of the response family; the fibre identification
  stated as an open problem
- **O19**: canonical amplitude normalisation derived

Thus:

- the observable is structurally motivated (its fibre reading remains an open bridge)
- the amplitude is now stripped of residual pipeline dependence

This is the final normalisation step before the physical interpretation of the
spectral window and the full fibre-level \(\delta\to\beta^*\) derivation.


# What O19 Adds

- explicit definition of the normalisation factor \(D(c,b_1,b_2,n)\)
- explicit distinction between \(\Sigma^{(c)}(n)\) and \(\sigma_c(n)\)
- phase-invariance analysis of the Gram–Schmidt residual increment
- formal basis test (P2) and block-instance test (P3)
- three-way classification of the residual factor \(r(c,q)\)
- mixed-factor decomposition
  \[
  r = r_{\mathrm{base}}\,r_{\mathrm{inst}}
  \]
  when required
- construction of a canonical pair observable
  \[
  \sigma_{\mathrm{pair}}^{\mathrm{can}}(n)
  \]
- proof that the exponent is unchanged by all canonicalisations considered


# Outcome

The spectral admissibility framework is now:

- parity-equivariant at the Born–Infeld level (**O18**), with the fibre identification open
- amplitude-level canonical (**O19**)
- free of residual pipeline ambiguity at the observable level

The pair observable is now:

- structurally motivated (fibre identification open, O18 Problem 2.8)
- canonically normalised


# Residual Open Problems

The main remaining questions are now:

1. **Spectral window selection (O20)**  
   Explain the restriction to \([7.4,10.6]\) through a dynamical persistence criterion

2. **Full \(\delta_{\mathrm{pair}}\to\beta^*\) derivation (O21)**  
   Derive the relation at the fibre level without pipeline assumptions

3. **Beyond the parity-pair framework**  
   Extend the analysis to enriched settings with additional admissible symmetries

4. **Generality beyond the current Weil/Heisenberg setting**  
   Determine how much of the normalisation structure persists in broader classes of
   admissibility models


# Status

The programme is now:

- observationally well-defined (**O17**)
- parity-equivariant, with the fibre identification stated as an open problem (**O18**)
- canonically normalised (**O19**)

Remaining work is now concentrated on:

- dynamical selection of the admissible exponent window
- full fibre-level cascade interpretation
- extension beyond the current spectral realisation


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
Canonical Normalisation of Pair Observables in Weil Blocks:
Eliminating Pipeline Dependence in the Gram–Schmidt Span Tracker,
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
