---
title: Coupled-branch families of AME states
description: Explicit AME families for 9, 11, 13, 15 and 17 parties in dimensions twice an odd prime power, with exact certificates and symmetric realizations.
layout: default
permalink: /research/ame/coupled-branch-families/
date_created: 2026-10-21
last_modified_at: 2026-10-25
---
<section class="page-head">
<p class="eyebrow">Research note · Manuscript in preparation</p>
<h1>Coupled-branch families of AME states</h1>
{% include page-dates.html %}
<p class="lede">Explicit AME families for 9, 11, 13, 15 and 17 parties in dimensions twice an odd prime power, obtained by coupling binary and finite-field quantum systems.</p>
</section>

<article class="prose">

<p>This note summarizes the constructions and certificates accompanying <em>Explicit absolutely maximally entangled states in dimensions twice a prime power</em>, a manuscript in preparation. The current results extend the original announcement to five families and include \(\operatorname{AME}(15,18)\).</p>

<h2>Five infinite families</h2>
<p>For every <strong>odd prime power</strong> \(q\) in the indicated range, the construction gives an \(\operatorname{AME}(N,2q)\) state. Here \(K\) is the number of coupled binary branches.</p>
<div class="research-table-wrap" role="region" aria-label="AME families and stored exact examples" tabindex="0">
<table class="research-table">
<thead><tr><th scope="col">Parties \(N\)</th><th scope="col">Odd prime powers \(q\)</th><th scope="col">Branches \(K\)</th><th scope="col">Stored examples: \(d=2q\)</th></tr></thead>
<tbody>
<tr><th scope="row">9</th><td>\(q\ge 5\)</td><td>4</td><td>10, 14, 18, 22, 26</td></tr>
<tr><th scope="row">11</th><td>\(q\ge 5\)</td><td>2</td><td>10, 14, 18, 22, 26</td></tr>
<tr><th scope="row">13</th><td>\(q\ge 17\)</td><td>16</td><td>34, 38, 46</td></tr>
<tr><th scope="row">15</th><td>\(q\ge 9\)</td><td>8</td><td>18, 22, 26, 34, 38, 46</td></tr>
<tr><th scope="row">17</th><td>\(q\ge 67\)</td><td>64</td><td>134</td></tr>
</tbody>
</table>
</div>
<p>The table contains 20 stored examples. Three additional reconstructions, \(\operatorname{AME}(7,10)\), \(\operatorname{AME}(7,14)\) and \(\operatorname{AME}(7,22)\), bring the certificate catalogue to <strong>23 coupled examples</strong>. These seven-party parameters are already covered by the work of Shi and collaborators <a href="#ref-shi">[1]</a>.</p>
<p>The fifteen-party family uses one binary ingredient with finite-field parents at \(q=9,11,13\), and Cauchy parents for all odd prime powers \(q\ge17\). Its smallest listed dimension is therefore 18; restricting to prime \(q\) gives a threshold of 11 and local dimension 22. The ranges above are sufficient for these constructions and do not assert general nonexistence below them.</p>

<h2>Construction in brief</h2>
<p>Write \(N=2k+1\) and identify each local space with \(\mathbb C^2\otimes\mathbb C^q\). The state is a coherent sum</p>
<div class="family-equations">
\[
|\Psi\rangle=\frac{1}{\sqrt K}\sum_{a=0}^{K-1}|u_a\rangle\otimes|v_a\rangle.
\]
</div>
<p>The binary branches \(|u_a\rangle\) have maximally mixed \(k\)-party marginals <em>on average</em>. The finite-field branches \(|v_a\rangle\), obtained by conditioning one site of an even-party AME parent, have maximally mixed \(k\)-party marginals and zero reduced cross terms between distinct branch labels on every such subsystem. Pairing the binary and finite-field degrees of freedom at each site therefore gives a pure state with every \(k\)-party marginal equal to \(I/(2q)^k\).</p>
<p>The infinite ranges follow from the coupling identity and a finite-field Cauchy determinant argument, together with the certified small-field parents. For extension fields, the graph phases use the field trace to the prime subfield.</p>

<h2>Nine-party existence in every dimension from three</h2>
<p>The nine-party family, explicit prime-power graph states, Reed–Solomon constructions, and Kitamura's \(\operatorname{AME}(9,6)\) input <a href="#ref-kitamura96">[6]</a> combine under partywise tensor products to give</p>
<div class="family-equations">
\[
\operatorname{AME}(9,d)\text{ exists}\quad\Longleftrightarrow\quad d\ge3,
\qquad d\in\mathbb Z,\ d\ge2.
\]
</div>
<p>Prime-power factors cover odd dimensions and dimensions divisible by four. For \(d=2m\) with \(m\) odd, one uses an \(\operatorname{AME}(9,6)\) factor when \(3\mid m\), or an \(\operatorname{AME}(9,2p)\) factor for a prime \(p\ge5\) dividing \(m\), then tensors the remaining factors. The binary case \(d=2\) is excluded by the known AME bounds <a href="#ref-scott">[7]</a>, also reproduced by an exact shadow calculation in the companion code.</p>

<h2>Exact certificates and symmetric realizations</h2>
<p>The 23 coupled examples are supported by exact binary-ingredient checks and <strong>142,226 oriented balanced-cut checks of their parent states</strong>, or 71,113 cuts after identifying opposite orientations. These finite certificates use integer, rational and finite-field arithmetic. The analytic arguments establish the infinite families; numerical marginal checks provide additional corroboration.</p>
<p>Isometries on the branch labels also permit symmetric realizations. Exact cyclotomic certificates include an \(\operatorname{AME}(15,62)\) state with a \(C_{15}\) party subgroup, and the accompanying proof gives an \(\operatorname{AME}(15,2p)\) realization with this subgroup for every prime \(p\equiv1\pmod{15}\). The party permutations are accompanied by local Clifford operations. These are certified symmetry subgroups; full group classifications are restricted to the specified factorwise Clifford class for eight original states.</p>

<h2>Contribution and context</h2>
<p>The contribution is the explicit small binary ingredients, effective prime-power thresholds, exact certificates and symmetric realizations. Coupling has precedents in Shi–Zhang–Zhao–Li <a href="#ref-shi">[1]</a>, Atlas <a href="#ref-atlas">[2]</a> and Kitamura <a href="#ref-kitamura1110">[3]</a>; parent and code constructions are also drawn from Bevins–Bidav <a href="#ref-bevins">[4]</a> and Hontarenko–Życzkowski <a href="#ref-hontarenko">[5]</a>. The enlarged family is presented without a claim of publication priority. Bounds on the binary ingredients and on branch capacity concern this coupling mechanism; they do not establish unrestricted AME nonexistence.</p>

<div class="notice"><strong>Manuscript in preparation.</strong> This update reflects the companion repository of 22 October 2026. The <a href="https://github.com/palashpandya/coupled-branch-ame">companion code and data</a> are currently private, at version 0.1 (pre-release). A public release and publication identifier will be linked when available.</div>

<h2>Selected references and prior constructions</h2>
<ol class="publication-list">
<li id="ref-shi">Shi, Zhang, Zhao and Li. <a href="https://arxiv.org/abs/2608.01011v1">arXiv:2608.01011</a>. Coupling binary and odd-dimensional branches.</li>
<li id="ref-atlas">Atlas. <a href="https://github.com/niketp03/atlas-fc-verified/blob/15e4b3a7584e218cec531aeaf71cce72a8a9ecb1/AtlasFCSolutions/Oqp35.lean">AME(9,10) construction</a>, pinned source.</li>
<li id="ref-kitamura1110">Kitamura. <a href="https://github.com/KitaKen1/ame-11-10-lean/tree/6b7d009a43970587a3386b690221bec4339ce271">AME(11,10) construction</a>, pinned source.</li>
<li id="ref-bevins">Bevins and Bidav. <a href="https://arxiv.org/abs/2608.05781v2">arXiv:2608.05781</a>. Parent and code constructions.</li>
<li id="ref-hontarenko">Hontarenko and Życzkowski. <a href="https://arxiv.org/abs/2609.11796v1">arXiv:2609.11796</a>. Finite-field parent constructions.</li>
<li id="ref-kitamura96">Kitamura. <a href="https://github.com/KitaKen1/ame-9-6-lean/tree/500ee827dffbeed9bb2ed502adcd6690943a7463">AME(9,6) construction</a>, pinned source used in the nine-party existence result.</li>
<li id="ref-scott">A. J. Scott. <a href="https://arxiv.org/abs/quant-ph/0310137">Multipartite entanglement, quantum-error-correcting codes, and entangling power of quantum evolutions</a>. Background and binary AME bounds.</li>
</ol>

<p><a class="link-arrow" href="{{ '/research/ame/' | relative_url }}">← Back to AME research</a></p>
</article>

