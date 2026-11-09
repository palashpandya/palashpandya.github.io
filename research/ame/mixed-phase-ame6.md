---
title: Mixed-phase AME(9,6) and AME(7,6) states
description: Exactly certified mixed binary/ternary phase states, local-unitary inequivalence, and continuous families for seven and nine six-level systems.
layout: default
permalink: /research/ame/mixed-phase-ame6/
date_created: 2026-11-09
last_modified_at: 2026-11-09
---
<section class="page-head">
<p class="eyebrow">Research note · Manuscript in preparation</p>
<h1>Mixed-phase AME states in local dimension six</h1>
{% include page-dates.html %}
<p class="lede">Exactly certified AME(9,6) and AME(7,6) states, local-unitary invariants, and continuous families of seven and nine six-level systems.</p>
</section>

<article class="prose">

<p>This note summarizes <em>Inequivalent and continuous families of absolutely maximally entangled states of seven and nine six-level systems</em>, a manuscript in preparation. The project studies how many essentially different states can be constructed at these parameters and which of them admit continuous deformations. Its <a href="#materials">companion research package</a> combines a seeded constructor, exact certificates, invariant calculations, and numerical corroboration.</p>

<h2>A mixed binary/ternary phase construction</h2>
<p>Each local six-level system is written as a qubit and a qutrit, with basis label \(z=3x+y\), where \(x\in\{0,1\}\) and \(y\in\mathbb F_3\). The state has flat amplitudes with phases</p>
<div class="family-equations">
\[
\psi(x,y)=6^{-N/2}(-1)^{q_G(x)}\omega^{q_C(y)+x^{\mathsf T}By+q_H(x)},
\qquad \omega=e^{2\pi i/3}.
\]
</div>
<p>Here \(q_M(u)=\sum_{i\lt j}M_{ij}u_i u_j\). The binary graph \(G\), ternary graph \(C\), coupling matrix \(B\), and logical phases \(H\) determine the state. The constructor takes the number of parties, local dimension, and a random seed; it does not take a known AME state as input. It searches for the graph ingredients and solves the remaining phase constraints exactly.</p>

<h2>313 exactly certified state records</h2>
<div class="research-table-wrap" role="region" aria-label="Certified mixed-phase state records and construction attempts" tabindex="0">
<table class="research-table">
<thead><tr><th scope="col">State</th><th scope="col">Certified records</th><th scope="col">Attempts</th><th scope="col">Balanced cuts per state</th></tr></thead>
<tbody>
<tr><th scope="row">AME(9,6)</th><td>213</td><td>220</td><td>126</td></tr>
<tr><th scope="row">AME(7,6)</th><td>100</td><td>100</td><td>35</td></tr>
</tbody>
</table>
</div>
<p>All <strong>313 distinct records</strong> pass exact finite-field AME certificates on every balanced bipartition. For nine parties, seed 507 gives 19 successes from 20 attempts, and seeds 1101–1108 give another 194 from 200. For seven parties, seed 507 gives 100 successes from 100 attempts.</p>
<p>The certificates use integer and finite-field arithmetic, without a floating-point threshold. Dense reduced-density-matrix calculations provide additional numerical checks on the states and cuts examined. The package also checks reproduction from seeds and indices, including the bounded-search misses.</p>

<h2>Distinguishing local-unitary classes</h2>
<p>A degree-eight invariant built from the realignment of reduced density matrices separates states that cannot be related by local unitaries. Exact averages over the 315 partitions of type \(1|4|4\) distinguish all <strong>19 seed-507 AME(9,6) states</strong>, even when party permutations and complex conjugation are allowed. Their invariant values also differ from that of <a href="https://github.com/KitaKen1/ame-9-6-lean/tree/500ee827dffbeed9bb2ed502adcd6690943a7463">Kitamura’s AME(9,6) state</a>.</p>
<p>Among the 100 AME(7,6) records, exact invariant calculations establish <strong>at least 99 local-unitary classes</strong>; one pair remains unresolved. The number of distinct records is therefore separate from the number of proven inequivalent classes.</p>

<h2>Continuous families</h2>
<p>Three explicit one-parameter AME(9,6) constructions have the form</p>
<div class="family-equations">
\[
|\psi(t)\rangle=e^{itZ_iZ_j}|\psi_0\rangle,\qquad t\in\mathbb R,
\]
</div>
<p>where \(Z_i\) acts on the binary factor at site \(i\). Exact certificates show that every point is AME. A nonconstant exact Laurent polynomial for the averaged invariant shows that each construction meets a continuum of local-unitary classes. Rigorous bounds separate every point of these families from Kitamura’s reference state.</p>
<p>The relation between the first two families, F1 and F2, remains open: their computed invariant polynomials coincide. F3 has a different polynomial, but its invariant range overlaps theirs. These calculations do not establish three mutually inequivalent families.</p>

<h2>Deformation directions and their scope</h2>
<p>An exact free-edge rule determines when a two-site binary phase preserves the AME conditions for all real angles. In the nine-party dataset it identifies the three family bases. The seven-party study includes a steered two-parameter construction and further phase and amplitude deformations.</p>
<p>The tangent calculations concern a specified ansatz with fixed \(C\) and \(B\). A tangent-kernel dimension does not by itself establish that all directions integrate jointly, and rigidity within this ansatz does not imply rigidity under arbitrary AME deformations.</p>

<h2 id="materials">Reproducibility and materials</h2>
<p>The <a href="https://github.com/palashpandya/mixed-phase-ame6">mixed-phase-ame6 companion repository</a> contains state records, exact certificates, invariant evaluators, reconstruction scripts, and numerical checks. Code is licensed under MIT; data and results under CC BY 4.0. This note reflects its README and manuscript draft at <a href="https://github.com/palashpandya/mixed-phase-ame6/tree/ba3554b5db5aeedf3060fedbe93862b8f7dd638e">the 9 November 2026 source revision</a>.</p>

<div class="notice"><strong>Manuscript in preparation.</strong> The companion repository is currently private, at version 0.1 (pre-release); its links require repository access. A public release and publication identifier will be linked when available.</div>

<p><a class="link-arrow" href="{{ '/research/ame/' | relative_url }}">← Back to AME research</a></p>
</article>
