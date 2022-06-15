---
marp: false
theme: poster
paginate: false
size: 33:50
math: katex
---

<!-- Start header -->
<div class="header">

<!-- Image in the upper left -->
<div>

![headerlogo](./images/hopkins-logo.png)

</div>

<!-- Title and author information -->
<div>

# Statistical Modeling of Structural Connectomes Reveal Heritability

## Jaewon Chung<span class=super>1\*</span>, Eric Bridgeford<span class=super>1</span>, Michael Powell<span class=super>1</span>, Joshua T. Vogelstein<span class=super>1</span>

##### 1 - Johns Hopkins University, $\ast$ - correspondence: ![icon](./images/email.png) [_j1c@jhu.edu_](mailto:j1c@jhu.edu) ![icon](./images/github.png) [_@j1c(Github)_](https://github.com/j1c) ![icon](./images/twitter.png) [_@j1chung(Twitter)_](https://twitter.com/j1chung)

</div>

<!-- Image on the upper right -->
<div>

![headerlogo](./images/nd_logo.png)

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

</div>
<div>

- Brain connectivity is \textbf{more similar in identical twins} compared to those of fraternal twins, siblings, and unrelated in all three models.

</div>
<div>

- Existing methods ignore spatial arrangement of the brain and are not statistically justified.

</div>
<div>

- Random graph theory and statistical approach enable formulation and testing of different models of connectome heritability.

</div>
<div>

- Stochastic ordering of similarity, from most similar to least similar, in identical, fraternal twins, siblings and unrelated people.

</div>

<!-- End columns-box -->
</div>
<!-- End box -->
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

![](./ohbm22/overview.png)
**Fig 1:** Overview of the framework for measuring heritability of connectomes.

## Do changes in genome cause changes in connectomes?

![w:1000px center](./ohbm22/dag.png)
**Fig 2:** Overview of the framework for measuring heritability of connectomes.

<br>

**_Human Connectome Project 1200_**

|            | Monozygotic  |  Dizygotic  | Non-twin siblings |
| :--------: | :----------: | :---------: | :---------------: |
|     N      |     322      |     212     |        490        |
|    Sex     | 196 F, 126 M | 125 F, 87 M |   237 F, 253 M    |
| Age (mean) |  29.6 (3.3)  | 28.9 (3.4)  |    28.3 (3.9)     |

### Different Statistical Models of Connectomes

![](./ohbm22/Illustrative_example.png)
**Fig X:** Illustrative examples

- **Exact:** Are they the same?
- **Global scale:** Are they same after considering global differences?
- **Vertex scale:** Are they same after considering edge wise differences?

<!-- End main column 1 -->
</div>

<!-- Start main column 2 -->
<div>

### Examining Distribution

![](./ohbm22/distributions.png)
**Fig X:** Distributions examples

### Examining Different Parcellation

![](./ohbm22/results.png)
**Fig X:** All parcellations examples

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

![left h:1in](./ohbm22/graspologic-logo.svg)

</div>
<div>

<!-- Badges for a package -->

[![h:.4in](https://pepy.tech/badge/graspologic)](https://pepy.tech/project/graspologic)
[![h:.4in](https://img.shields.io/github/stars/microsoft/graspologic?style=social)](https://github.com/microsoft/graspologic)

</div>
<div>

<!-- QR code to a package -->

![center h:1in](./ohbm22/graspologic-qr.svg)

</div>
</div>

<div class="columns3-np">
<div>

<!-- Logo for a package -->

<p style="text-align: center;">

**hyppo**

</p>

</div>
<div>

<!-- Badges for a package -->

[![h:.4in](https://pepy.tech/badge/hyppo)](https://pepy.tech/project/hyppo)
[![h:.4in](https://img.shields.io/github/stars/neurodata/hyppo?style=social)](https://github.com/neurodata/hyppo)

</div>
<div>

<!-- QR code to a package -->

![center h:1in](./ohbm22/hyppo-qr.svg)

</div>
</div>

<br>

#### Acknowledgements

<footer>
NeuroData lab for many ideas and feedback. Many at Microsoft Research for w/ graspologic.
</footer>

</div>
<div>

#### References

<!-- Need these breaks <br> between refs otherwise formatting breaks for some reason -->
<footer>
[1] Chung et al. "The complete connectome of an insect brain," In preparation (2022)
<br>
[2] Chung et al. "Statistical connectomics," Ann. Rev. Statistics and its Application (2021)
<br>
[3] Athreya et al. "Statistical inference on random dot product graphs: a survey," JMLR (2017)
</footer>

#### Funding

<footer>
J.C. supported by the BRAIN Initiative (1RF1MH123233). J.T.V. supported by NSF CAREER Award (1942963). Findings and conclusions expressed are  those of the authors and not necessarily those of the funders.
</footer>

</div>
</div>

<!-- End main column 2 -->
</div>

<!-- End main columns -->
</div>
