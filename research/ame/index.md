---
title: Absolutely maximally entangled states
description: Definitions and selected public research on AME states.
layout: default
date_created: 2026-10-08
last_modified_at: 2026-10-21
permalink: /research/ame/
---
<section class="page-head">
<p class="eyebrow">Research / Multipartite entanglement</p>
<h1>Absolutely maximally entangled states</h1>
{% include page-dates.html %}
<p class="lede">Mathematical structures at the intersection of multipartite entanglement, quantum error correction, and numerical optimization.</p>
</section>
<article class="prose">
<h2>Definition</h2>
<p>A pure state \(|\psi\rangle\in(\mathbb C^d)^{\otimes n}\) is absolutely maximally entangled, denoted AME\((n,d)\), if each reduction to \(\lfloor n/2\rfloor\) parties is maximally mixed:</p>
<p>\[\rho_A=\operatorname{Tr}_{A^c}(|\psi\rangle\langle\psi|)=\frac{I_{d^{|A|}}}{d^{|A|}},\qquad |A|=\lfloor n/2\rfloor.\]</p>
<p>Reductions on smaller subsets are then maximally mixed as well. The existence and explicit construction of such states depend on the number of parties and their local dimension.</p>
<h2>Why study them?</h2>
<p>AME states connect multipartite entanglement to quantum error-correcting codes, combinatorial designs, and multiunitary structures. These connections provide complementary algebraic, geometric, and computational ways to study existence and construction problems.</p>
<h2>Computational viewpoint</h2>
<p>One diagnostic is the sum of squared deviations from maximal mixing across the relevant bipartitions:</p>
<p>\[\mathcal L(\psi)=\sum_{|A|=\lfloor n/2\rfloor}\left\|\rho_A-\frac{I}{d^{|A|}}\right\|_F^2.\]</p>
<p>For normalized pure states, \(\mathcal L(\psi)=0\) if and only if the state is AME. Finding low values numerically is not by itself an existence proof; careful validation is essential.</p>
<h2>Coupled-branch AME families (2026)</h2>
<p>Previously unreported families of AME(13,2p), AME(15,2p), and AME(17,2p) states using an established coupling approach. The constructions include eight exactly certified examples and the exceptional AME(15,26) state. Manuscript in preparation.</p>
<p><a class="link-arrow" href="{{ '/research/ame/coupled-branch-families/' | relative_url }}">Read the coupled-branch note →</a></p>
<h2>Selected research: real AME(4,6) states</h2>
<p>A 60-term real AME(4,6) construction with a block-orthogonal description, closed-form continuous families, and a classification of 4,096 real states into 20 equivalence classes on two associated supports. The manuscript is in preparation, and <a href="https://github.com/palashpandya/real-ame46">the companion code and data are public</a>.</p>
<p><a class="link-arrow" href="{{ '/research/ame/real-ame46/' | relative_url }}">Read the research note →</a></p>
<p><a class="link-arrow" href="{{ '/research/' | relative_url }}">← All research areas</a></p>
</article>