---
marp: true
theme: poster
paginate: false
size: 33:44
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
- Brain connectivity is \textbf{more similar in identical twins} compared to those of fraternal twins, siblings, and unrelated in all three models.

</div>

<!-- Box col2 -->
<div>

- Existing methods ignore spatial arrangement of the brain and are not statistically justified.

</div>

<!-- Box col3 -->
<div>

- Random graph theory and statistical approach enable formulation and testing of different models of connectome heritability.

</div>

<!-- Box col4 -->
<div>

- Stochastic ordering of similarity, from most similar to least similar, in identical, fraternal twins, siblings and unrelated people.

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

![](./ohbm22/overview.png)
**Fig 1:** Overview of the framework for measuring heritability of connectomes.

## Do changes in genome cause changes in connectomes?

### Thing we did 1

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sodales quam sed felis fringilla cursus. Morbi nec finibus massa. Aenean varius cursus enim vitae sagittis. Proin dictum, erat vitae sollicitudin porttitor, felis risus gravida tortor, vel placerat sem magna eget enim. Aliquam pretium nulla in ultrices venenatis. Nunc sit amet mi gravida, scelerisque turpis ullamcorper, luctus quam. Mauris consequat laoreet nibh a sagittis. Fusce porta, dui sed gravida lacinia, massa tellus varius ante, sit amet sodales erat justo aliquam nulla. Suspendisse commodo finibus nisi quis laoreet. Donec vitae felis volutpat, convallis lectus tincidunt, vestibulum eros.

### Thing we did 2

Aliquam sed finibus lacus. In ut nibh mollis, viverra dolor ac, egestas urna. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Aliquam erat volutpat. Praesent vel condimentum est. Ut vitae velit lacinia, dignissim augue sit amet, bibendum eros. Aliquam erat volutpat. Nam nec suscipit eros.

<!-- End main column 1 -->
</div>

<!-- Start main column 2 -->
<div>

### Thing we did 3

<!-- ![](../../../results/figs/thresholding_tests/edge_weight_dist_input_proportion.png) -->

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

<br>

<div class="columns3-np">
<div>

This work

</div>

</div>

#### Acknowledgements

<footer>
NeuroData lab for many ideas and feedback. Many at Microsoft Research for w/ graspologic.
</footer>

</div>
<div>

#### References

<!-- Need these breaks <br> between refs otherwise formatting breaks for some reason -->
<footer>
[1] Winding, Pedigo et al. "The complete connectome of an insect brain," In preparation (2022)
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
