---
title: Absolutely maximally entangled states
description: Definitions and selected public research on AME states.
layout: default
permalink: /research/ame/
---
<section class="page-head">
<p class="eyebrow">Research / Multipartite entanglement</p>
<h1>Absolutely maximally entangled states</h1>
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
<h2>Selected result: a real AME(4,6) state</h2>
<p>An explicit real AME(4,6) construction with 60 non-zero coefficients. A manuscript is in preparation.</p>
<p><a class="link-arrow" href="{{ '/research/ame/real-ame46/' | relative_url }}">Read the short announcement →</a></p>
<div class="notice"><strong>Publication scope.</strong> Only selected high-level research summaries appear here. Detailed constructions and numerical data will be shared after review; the working repository remains private.</div>
<p><a class="link-arrow" href="{{ '/research/' | relative_url }}">← All research areas</a></p>
</article>