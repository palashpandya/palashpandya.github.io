---
title: Real AME(4,6) states
description: A real 60-term AME(4,6) construction, continuous families and a classification of real states.
layout: default
date_created: 2026-10-08
last_modified_at: 2026-10-21
permalink: /research/ame/real-ame46/
---
<section class="page-head">
<p class="eyebrow">Research preprint · <a href="https://arxiv.org/abs/2610.16673">arXiv:2610.16673</a></p>
<h1>Real AME(4,6) states</h1>
{% include page-dates.html %}
<p class="lede">A real solution of Euler's thirty-six officers problem, with a simple orthogonal block structure, continuous families and a classification of related real states.</p>
</section>

<article class="prose">

<p>This page summarizes the preprint <em>Euler's thirty-six officers need not all be entangled: real AME(4,6), families and classification</em>. The <a href="https://github.com/palashpandya/real-ame46">companion repository</a> is public and contains the manuscript source, exact state data and verification scripts.</p>

<h2>The real state</h2>
<p>We construct a pure state of four six-level systems (quhexes) whose coefficients are real and whose two-party reduced states are all maximally mixed:</p>
<p>\[
\rho_{AB}=\frac{I_{36}}{36}\qquad\text{for every pair of parties }A,B.
\]</p>

<p>In the computational basis it has <strong>60 non-zero coefficients</strong>: 30 equal to \(+1/\sqrt{72}\), 18 equal to \(-1/\sqrt{72}\), and 12 equal to \(+\sqrt{2}/\sqrt{72}=1/6\). The other 1,236 coefficients vanish.</p>

<p>For each of the three bipartitions, the corresponding \(36\times36\) reshaping of \(6\psi\) is real orthogonal. After permuting rows and columns, it consists of <strong>12 scalar \(1\times1\) blocks</strong> and <strong>12 orthogonal \(2\times2\) blocks</strong>. In the thirty-six officers interpretation, this gives 12 classical officers and 24 entangled, two-term officers.</p>

<figure class="ame-figure">
<div class="ame-diagram-scroll" role="region" aria-label="Color-coded amplitudes for the three AME(4,6) bipartitions" tabindex="0">
<img src="{{ '/assets/illustrations/real-ame46-amplitudes.svg' | relative_url }}" alt="The three color-coded 36-by-36 coefficient matrices in natural order, and beneath them the same matrices permuted into twelve scalar and twelve orthogonal two-by-two blocks. Blue is minus one, red is plus one, and dark red is plus square root of two after scaling by square root of 72." width="960" height="713" loading="lazy">
</div>
<figcaption>The three reshapings of \(\sqrt{72}\,\psi\). Blue denotes \(-1\), red \(+1\), dark red \(+\sqrt{2}\), and white zero. The lower row makes the \(1\times1\) and \(2\times2\) orthogonal blocks visible. <a href="{{ '/assets/illustrations/real-ame46-amplitudes.svg' | relative_url }}" target="_blank" rel="noopener noreferrer">Open the full-size figure ↗</a></figcaption>
</figure>

<h2>Continuous families and real-state classification</h2>
<p>The construction lies at the boundary of a <strong>72-term family</strong> of AME(4,6) states, with two complex-conjugate components, each having 10 parameters modulo diagonal local unitaries. Some members have uniform non-zero amplitude magnitudes. At the two endpoints, the support drops to 60 terms, giving two 11-parameter families.</p>

<p>On these two 60-term supports there are <strong>4,096 real AME states</strong>, counted up to diagonal local unitaries. Of these, 1,024 are limits of the 72-term family. Under arbitrary local unitaries and permutations of the parties, the real states fall into <strong>exactly 20 equivalence classes</strong>: eight on one support and twelve on the other. The separation of the classes is certified using interval arithmetic.</p>

<h2>How the construction arose</h2>
<p>The state emerged from a search restricted to an eigenspace of a finite-order local symmetry, \(u^{\otimes4}\), with \(u=\operatorname{diag}(i,-1,-1,-i,-i,-i)\). Minimizing the support in suitable local frames led to a 72-term orthogonal array of strength two. On this support, the AME conditions reduce to equations linear in squared amplitudes and phase congruences, yielding the closed-form families and their real boundary states.</p>

<h2>Context and materials</h2>
<p>Whether a real AME(4,6) state exists was posed as an open problem in a <a href="https://arxiv.org/abs/2508.04777">2026 review</a>. Independent real constructions have also been announced by W. Bruzda, S. A. Rather, and jointly by M. Hontarenko and K. Życzkowski, as acknowledged in the preprint. This work develops the 60-term construction, its classical-officer structure, continuous families and classification on the two associated supports.</p>

<p>The <a href="https://github.com/palashpandya/real-ame46/blob/main/README.md">updated technical report</a>, <a href="https://github.com/palashpandya/real-ame46/blob/main/paper/main.tex">manuscript source</a>, <a href="https://github.com/palashpandya/real-ame46/tree/main/results">verification results</a>, and <a href="https://github.com/palashpandya/real-ame46/tree/v1.0">version 1.0 of the companion code and data</a> are available on GitHub. Exact arithmetic establishes the state and the family relations; the classification also includes certified interval-arithmetic calculations.</p>

<div class="notice"><strong>Preprint available.</strong> Palash Pandya, <em>Euler's thirty-six officers need not all be entangled: real AME(4,6), families and classification</em>, <a href="https://arxiv.org/abs/2610.16673">arXiv:2610.16673</a> (2026; submitted 12 October 2026).</div>

<p><a class="link-arrow" href="{{ '/research/ame/' | relative_url }}">← Back to AME research</a></p>

</article>
