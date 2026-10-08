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
<p>In the computational basis, the normalized state has <strong>30 coefficients equal to \(+1/\sqrt{72}\)</strong>, <strong>18 equal to \(-1/\sqrt{72}\)</strong>, and <strong>12 equal to \(+\sqrt{2}/\sqrt{72}=1/6\)</strong>. The remaining 1,236 of the \(6^4=1296\) coefficients are zero.</p>

<figure class="ame-figure ame-structure">
<div class="ame-structure-lead">Three bipartitions of the four parties</div>
<div class="ame-structure-pairings" aria-label="Three bipartitions: 12 versus 34, 13 versus 24, and 14 versus 23">
<span>12 | 34</span>
<span>13 | 24</span>
<span>14 | 23</span>
</div>
<div class="ame-structure-flow">↓ &nbsp; Reshape to 36 × 36; independently permute rows and columns</div>
<div class="ame-block-types">
<div class="ame-block-type">
<div class="ame-block-math">\([1]\)</div>
<div class="ame-block-label"><strong>12</strong> scalar blocks (1 × 1)</div>
</div>
<div class="ame-block-sum" aria-hidden="true">⊕</div>
<div class="ame-block-type">
<div class="ame-block-math">\(\frac{1}{\sqrt{2}}\begin{pmatrix}1&1\\1&-1\end{pmatrix}\)</div>
<div class="ame-block-label"><strong>12</strong> orthogonal blocks (2 × 2)</div>
</div>
</div>
<figcaption>Common block structure of all three reshapings, shown schematically. The 2 × 2 block is one representative signed pattern; the actual blocks may have different signs. No coefficient positions are shown.</figcaption>
</figure>

<h2>Why it matters</h2>
<p>Earlier AME(4,6) constructions used complex coefficients. A real construction was posed as an open question in a <a href="https://arxiv.org/abs/2508.04777">recent review</a>; the existence of an orthogonal two-unitary of order 36 had also been conjectured to be impossible. </p>

<h2>Beyond the example</h2>
<p>The state is not isolated within the space of complex AME states. The manuscript describes two continuous families passing through it and a classification of related real solutions.</p>

<div class="notice"><strong>To be published soon.</strong> This result is currently unpublished. The explicit state, proof, and details of the families will be presented in the forthcoming manuscript.</div>

<p><a class="link-arrow" href="{{ '/research/ame/' | relative_url }}">← Back to AME research</a></p>

</article>
