# DEBRIEF-math-erdos1061

A DEBRIEF mission record (protocol https://github.com/Nervous-Machine/DEBRIEF) for **The claimed solution of Erdős Problem #1061 (solutions of sigma(a) + sigma(b) = sigma(a+b))**.

This claim is on the public claims board, https://math-board.nervousmachine.com, which shows its stage, who has contributed, and what it needs next.

**Standing.** Certified 0. Accepted 0. Refuted 0. Open gaps 2. This record is at tier zero: the claim and its public artifacts are pinned, the checks still owed are listed, and nothing has been run or read yet. The first contribution is open.

## The problem

Let sigma(n) be the sum of the divisors of n. Count the pairs of positive integers a, b with a + b at most x such that sigma(a) + sigma(b) = sigma(a + b). Is the count asymptotic to c times x for some constant c, or is it of higher order?

Source: https://www.erdosproblems.com/1061 (posed: a question of Erdős reported as problem B15 in Guy's collection (2004)).

A third-party formalization of the problem statement exists: `FormalConjectures/ErdosProblems/1061.lean` in github.com/google-deepmind/formal-conjectures at commit `e028240a61822d970c933f4656f51da025cf200b` (blob `54fc67ce424652d144268e7a639b793b9934ebef`). It is the natural reference for whether a claimant's Lean theorem states this problem.

## The claim

**Eric Li**, using GPT-5.5 Pro (as listed by the claimant), submitted 2026-07-26 at https://www.erdosproblems.com/forum/thread/1061/proof-claims.

The claim is that the count S(x) grows faster than x times any fixed power of log x, so the linear asymptotic fails in the higher-order direction. The construction starts from three integers with the same abundancy index, reduces the identity to two equations in six primes lying on a split quadric, parametrises the quadric rationally, and counts prime points on the resulting planes with a sieve and a higher-dimensional Siegel–Walfisz theorem. The author notes that Guy's phrasing asks whether the count is cx + o(x) or of higher order, so a precise asymptotic is not required.

Artifacts, pinned:

- an arXiv preprint: arXiv:2606.25849v1 "A resolution of Erdős Problem 1061 on the sum-of-divisors function" (published 2026-06-24, last revised 2026-06-24)

Status on the problem page as of 2026-11-14: listed as one proof claim; not marked accepted by the site.

## What is owed

Each open gap is in `ASKS.md` with what closes it and who could act. In order:

1. **No formal deduction exists for the claimed proof** (EG1): A formalization of the main theorem, with the statement written by someone other than the prover.
2. **No independent mathematician has reported reading the proof, and there is no referee report** (EG2): Someone in the field reads it and says, under their name, what holds and what does not.

## Contributing

- **Rerun** (if there is a Lean development): copy `prereg_rerun.yaml`, fill in your predictions, register it with `tools/prereg.py register` from the protocol repository and commit it *before* running anything. Run. Report with the **Rerun report** issue form; it becomes a `rerun` cycle under your name.
- **Read**: a trace (reading guide) does not exist yet. Writing one is itself a `trace` cycle. Once it exists, the **Semantic read** form takes signatures and refusals.
- **Anything else**: open a plain issue.

Rules and templates: https://github.com/Nervous-Machine/DEBRIEF/blob/main/CONTRIBUTING.md. Every contribution is one dated cycle under your own name and goes into `CITATION.cff` and the next release.

## Layout

```
ledger/erdos1061.json   the ledger (protocol 0.1.0)
claim.yaml            the pinned claim this record was opened from
SCORECARD.md / ASKS.md  generated from the ledger
prereg_rerun.yaml     a pre-registration template for the first rerun (unregistered)
cycles/               contributed cycles, one file each
```

## Words

This record never calls the claim proved, verified or a theorem. It records what was claimed, what was checked by whom under what rule, and what is still open. Nothing here has standing until a cycle gives it one.
