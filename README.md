# Hardy–Weinberg Practice Lab

Open `index.html` in a web browser. The single file contains all styling, code, and graphics; no installation, server, or internet connection is required.

## Student flow

1. Choose genotype counts, allele frequency, or recessive phenotype and a difficulty level.
2. Calculate p, q, and expected AA, Aa, and aa frequencies independently.
3. Submit all five answers to reveal the graph and worked solution. The graph plots submitted genotype frequencies at the submitted p and correct frequencies at the correct p.
4. Answer an interpretation question or explore repeated random samples.
5. Generate another problem, or copy/reload a problem code to reproduce a question.

All levels accept an absolute error of ±0.005 (half a percentage point). Students can round final answers to two decimal places. Very small frequencies can therefore be accepted as 0.00; worked solutions retain more precision to distinguish a small frequency from true absence. A formula reminder is available before submission. Student answers are locked after submission and cleared by a new problem, code load, change of settings, or page reload.

## Teaching scope

One diploid locus with two alleles. Genotype-count questions derive allele frequencies directly from observed counts; these counts need not follow Hardy–Weinberg proportions. Recessive-phenotype questions explicitly assume Hardy–Weinberg equilibrium and that all and only aa individuals express the phenotype. Fractional expected counts are averages, not literal individuals. The sampling activity draws independent genotypes using fixed probabilities; it does not simulate evolution across generations or perform a significance test.

This is a practice tool. It does not save answers, identify students, or submit grades. Students can inspect client-side code or reload a question, so the reveal sequence is instructional rather than secure assessment enforcement.

## Verification

Run `node hardy_weinberg/check.cjs` from the BIS181 directory (or `node check.cjs` from this folder).

The check covers 9,000 generated problems, mathematical invariants, nonnegative integer counts, deterministic replay, all nine type/difficulty submission flows, answer locking, sampling, two-decimal answers across all levels and rejection of full credit for all-zero submissions, and invalid problem codes. The lifecycle checks use a minimal DOM substitute, not a browser.

Rendered layout and real-browser interaction remain unverified: the automated browser blocked the local file URL. The stylesheet includes responsive layouts, and the chart redraws to its container width.
