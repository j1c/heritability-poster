---
marp: true
theme: poster
paginate: false
size: 35:70
---

<!-- Start header -->
<div class="header">

<!-- Image in the upper left -->
<div>

![headerlogo](../images/hopkins-logo.png)

</div>

<!-- Title and author information -->
<div>

# Statistical Modelling of Structural Connectomes Reveal Heritability

## Jaewon Chung<span class=super>1\*</span>, Eric Bridgeford<span class=super>1</span>, Michael Powell<span class=super>1</span>, Joshua T. Vogelstein<span class=super>1</span>

##### 1 - Johns Hopkins University, $\ast$ - correspondence: ![icon](../images/email.png) [_j1c@jhu.edu_](mailto:j1c@jhu.edu) ![icon](../images/github.png) [_@j1c(Github)_](https://github.com/<insert-handle>) ![icon](../images/twitter.png) [_@j1chung(Twitter)_](https://twitter.com/<insert-handle>)

</div>

<!-- Image on the upper right -->
<div>

![headerlogo](../images/nd_logo.png)

</div>

<!-- End header -->
</div>

<!-- Summary box title -->

<span class='h3-noline'> Summary </span>

<!-- Summary box using 5 columns-->
<div class='box'>
<div class="columns-box">

<!-- Box col1 -->
<div>

- Understanding how brain connectivity is influenced by genetics can improve our understanding of brain function and diseases.
- Existing methods ignore spatial arrangement of the brain and are not statistically justified.
- Random graph theory and statistical approach enable formulation and testing of different models of connectome heritability.
- Brain connectivity is \textbf{more similar in identical twins} compared to those of fraternal twins, siblings, and unrelated in all three models.
- Stochastic ordering of similarity, from most similar to least similar, in identical, fraternal twins, siblings and unrelated people.
- Same framework is used to identify regions of the brain that contribute most to heritability.
- _graspologic_ - Open-source implementation of all algorithm used for this study.

</div>

<!-- Box col2 -->
<div>

- Current research on connectomics, specifically heritability, focus mostly on fMRI.

</div>

<!-- Box col3 -->
<div>

- Then we did this other awesome thing.

</div>

<!-- Box col4 -->
<div>

- Finally, we did this amazing thing.

</div>

<!-- End columns and box -->
</div>
</div>

<!-- Start main 2 column split for poster -->
<div class="columns-main">

<!-- Start main column 1 -->
<div>

### Motivation

- Connectomes are rich sources of inspiration for architectures in artificial intelligence.
- Comparing connectomes could help elucidate which structural features are necessary for yielding the capabilities animal intelligences.
- Bilateral symmetry for connectomes is one such comparison; has been investigated, but not clearly defined as a network hypothesis.

### What are we going to do

<!-- Big question for this work -->

## Are the <span style="color:var(--left)"> left </span> and <span style="color:var(--right)"> right </span> networks "different"?

<br>

This is what we need to do for this work

### Thing we did 1

<div class=columns2>
<div>

![](../../../results/figs/er_unmatched_test/er_methods.svg)

</div>
<div>

![](../../../results/figs/er_unmatched_test/er_density.svg)

</div>
</div>

<div class=columns2>
<div>

**Fig 2A:** Testing symmetry under Erdos-Renyi (ER) model [2] compares global connection probability (density), here via Fisher's exact test.

</div>
<div>

**Fig 2B:** Test comparing densities rejected ($p{<}10^{-23}$), even the simplest model parameter differs between hemispheres.

</div>
</div>

<!-- End main column 1 -->
</div>

<!-- Start main column 2 -->
<div>

### Thing we did 2

<div class="columns2">
<div>

<!-- Example of a table, here within a column split -->

#### With Kenyon cells

| Model |                       $H_0$ (vs. $H_A \neq$)                       |    p-value    |
| :---: | :----------------------------------------------------------------: | :-----------: |
| **1** |  $\color{#66c2a5} p^{(L)} \color{black} = \color{#fc8d62}p^{(R)}$  | ${<}10^{-23}$ |
| **2** | $\color{#66c2a5} B^{(L)} \color{black} = \color{#fc8d62} B^{(R)}$  | ${<}10^{-7}$  |
| **3** | $\color{#66c2a5}B^{(L)} \color{black}  = c \color{#fc8d62}B^{(R)}$ | ${<}10^{-2}$  |

</div>
<div>

#### Without Kenyon cells

| Model |                       $H_0$ (vs. $H_A \neq$)                       |    p-value    |
| :---: | :----------------------------------------------------------------: | :-----------: |
| **1** |  $\color{#66c2a5} p^{(L)} \color{black} = \color{#fc8d62}p^{(R)}$  | ${<}10^{-26}$ |
| **2** | $\color{#66c2a5} B^{(L)} \color{black} = \color{#fc8d62} B^{(R)}$  | ${<}10^{-2}$  |
| **3** | $\color{#66c2a5}B^{(L)} \color{black}  = c \color{#fc8d62}B^{(R)}$ |    $0.51$     |

</div>
</div>

### Thing we did 3

<!-- ![](../../../results/figs/thresholding_tests/edge_weight_dist_input_proportion.png) -->

<div class="columns2">
<div>

![](./results/thresholding_tests/../../../../../results/figs/thresholding_tests/thresholding_methods.svg)

</div>
<div>

![](../../../results/figs/thresholding_tests/input_threshold_pvalues_legend.svg)

</div>
</div>

<div class="columns2">
<div>

**Fig 5A:** Removed edges w/ weight (synapse count or percentage of input to downstream neuron) below some threshold, tested symmetry for each pair of networks.

</div>
<div>

**Fig 5B:** Did not detect asymmetry in networks of only top ~$50\%$ of edges (by input percentage) under models studied here. Not true using synapse counts edge weights (not shown).

</div>
</div>

### Limitations and extensions

- Other models to consider (e.g. random dot product graph [3])
- Other sensible neuron groupings for group connection test
- Matching nodes across networks leads to new models, likely more power

<!-- Code/Refs/Thanks/Funding - small section -->

###

<div class="columns2">
<div>

#### Code

<div class="columns3-np">
<div>

<!-- Logo for a package -->

![left h:1in](./../../images/graspologic_svg.svg)

</div>
<div>

<!-- Badges for a package -->

[![h:.4in](https://pepy.tech/badge/graspologic)](https://pepy.tech/project/graspologic)
[![h:.4in](https://img.shields.io/github/stars/microsoft/graspologic?style=social)](https://github.com/microsoft/graspologic)

</div>
<div>

<!-- QR code to a package -->

![center h:1in](./../../images/graspologic-qr.svg)

</div>
</div>

<br>

<div class="columns3-np">
<div>

This work

</div>
<div>

<!-- JupyterBook/Docs for a project -->

[![h:0.4in](https://jupyterbook.org/badge.svg)](http://docs.neurodata.io/bilateral-connectome/)

</div>
<div>

<!-- QR code to link to repo for a project -->

![center h:1in](./../../images/bilateral-qr.svg)

</div>
</div>

#### Acknowledgements

<footer>
Marta Zlatic's lab, Albert Cardona's lab and all tracers for the amazing dataset and many ideas. NeuroData lab for feedback. Many at Microsoft Research for w/ graspologic.
</footer>

</div>
<div>

#### References

<!-- Need these breaks <br> between refs otherwise formatting breaks for some reason -->
<footer>
[1] Winding, Pedigo et al. "The complete connectome of an insect brain," In preparation (2022)
<br>
[2] Chung et al. "Statistical connectomics," Ann. Rev. Statistics and its Application (2021) <br>
[3] Athreya et al. "Statistical inference on random dot product graphs: a survey," JMLR (2017)
</footer>

#### Funding

<footer>
B.D.P. supported by the NSF GRFP (DGE1746891). J.T.V. supported by NSF CAREER Award (1942963). J.T.V + C.E.P supported by NIH BRAIN Initiative (RF1MH123233). Findings and conclusions expressed are  those of the authors and not necessarily those of the funders.
</footer>

</div>
</div>

<!-- End main column 2 -->
</div>
<!-- End main columns -->
</div>
