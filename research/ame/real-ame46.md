---
title: A real AME(4,6) state
description: An unpublished construction of a real absolutely maximally entangled state of four six-level systems.
layout: default
permalink: /research/ame/real-ame46/
---
<section class="page-head">
<p class="eyebrow">Unpublished result · Manuscript in preparation</p>
<h1>A real AME(4,6) state</h1>
<p class="lede">An explicit absolutely maximally entangled state of four six-level quantum systems whose coefficients are all real.</p>
</section>

<article class="prose">

<h2>The result</h2>
<p>We have constructed a real pure state of four six-level systems (quhexes) whose every two-party reduced density matrix is maximally mixed:</p>

<p>\[
\rho_{AB}=\frac{I_{36}}{36}
\qquad \text{for every pair } A,B.
\]</p>

<p>The state has <strong>60 non-zero coefficients</strong> in the computational basis. Its amplitudes are real, and the corresponding three \(36\times36\) matrix reshapings are all orthogonal after multiplication by 6. This gives a real orthogonal two-unitary matrix of order 36.</p>

<h2>Real coefficients</h2>
<p>In the computational basis, the normalized state has three distinct nonzero real coefficients, with the following multiplicities:</p>
<div class="coeff-chart" aria-label="Counts of nonzero real amplitudes in the AME(4,6) state">
  <div class="coeff-row">
    <span class="coeff-value">\(+1/\sqrt{72}\)</span>
    <span class="coeff-track" aria-hidden="true"><span class="coeff-bar coeff-positive" style="width:100%"></span></span>
    <strong class="coeff-count">30</strong>
  </div>
  <div class="coeff-row">
    <span class="coeff-value">\(-1/\sqrt{72}\)</span>
    <span class="coeff-track" aria-hidden="true"><span class="coeff-bar coeff-negative" style="width:60%"></span></span>
    <strong class="coeff-count">18</strong>
  </div>
  <div class="coeff-row">
    <span class="coeff-value">\(+\sqrt{2}/\sqrt{72}=1/6\)</span>
    <span class="coeff-track" aria-hidden="true"><span class="coeff-bar coeff-root-two" style="width:40%"></span></span>
    <strong class="coeff-count">12</strong>
  </div>
</div>
<p>Thus 60 of the \(6^4=1296\) basis amplitudes are nonzero, while the remaining <strong>1,236 coefficients are zero</strong>. The counts give the exact normalization:</p>
<p>\[30\left(\frac{1}{\sqrt{72}}\right)^2+18\left(\frac{-1}{\sqrt{72}}\right)^2+12\left(\frac{1}{6}\right)^2=\frac{30+18+24}{72}=1.\]</p>

<figure class="ame-figure">
<img src="{{ '/assets/illustrations/real-ame46-blocks.svg' | relative_url }}" alt="A schematic of the three pairings 12 versus 34, 13 versus 24, and 14 versus 23. Each 36 by 36 orthogonal reshaping can be rearranged into twelve one by one blocks and twelve two by two blocks." width="960" height="335" loading="lazy">
<figcaption>Structure of the three bipartitions. After suitable row and column permutations, each reshaping decomposes into 12 scalar blocks and 12 orthogonal 2 × 2 blocks. This is a schematic, not a plot of the actual coefficients.</figcaption>
</figure>

<h2>Why it matters</h2>
<p>Earlier AME(4,6) constructions used complex coefficients. A real construction was posed as an open question in a <a href="https://arxiv.org/abs/2508.04777">recent review</a>; the existence of an orthogonal two-unitary of order 36 had also been conjectured to be impossible. To our knowledge, this construction gives the first real AME(4,6) state.</p>

<h2>Beyond the example</h2>
<p>The state is not isolated within the space of complex AME states. The manuscript describes two continuous families passing through it and a classification of related real solutions.</p>

<div class="notice"><strong>To be published soon.</strong> This result is currently unpublished. The explicit state, proof, and details of the families will be presented in the forthcoming manuscript.</div>

<p><a class="link-arrow" href="{{ '/research/ame/' | relative_url }}">← Back to AME research</a></p>

</article>
