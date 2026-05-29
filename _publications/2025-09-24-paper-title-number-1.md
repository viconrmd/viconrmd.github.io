---
title: "Masked Circuit Compiler in the Cardinal Random Probing Composability Framework"
collection: publications
category: conferences
layout: single
permalink: /publication/2025-09-24-paper-title-number-1
date: 2025-09-24
venue: 'Asiacrypt'
paperurl: 'https://eprint.iacr.org/2025/1747.pdf'
excerpt: "Sonia Belaïd, Victor Normand and Matthieu Rivain."
---

The random probing model formalizes a leakage scenario where each wire in a
circuit leaks with probability . This model holds practical relevance due to its
reduction to the noisy leakage model, which is widely regarded as the
appropriate formalization for power and electromagnetic side-channel attacks. 

In this paper, we present new techniques for designing efficient masking schemes
that achieve tighter random probing security with lower complexity. First, we
introduce the notion of *cardinal random probing composability*
(Cardinal-RPC), offering a new trade-off between complexity and security for
composing masking gadgets. Next, we propose a novel refresh technique based on a
simple iterative process: randomly selecting and updating two shares with fresh
randomness. While not perfectly secure in the standard probing model, this
method achieves arbitrary cardinal-RPC security, making it a versatile tool for
constructing random-probing secure circuits. Using this refresh, we develop
additional basic gadgets (e.g., linear multiplication, addition, and copy) that
satisfy the cardinal-RPC notion. Despite the increased complexity, the gains in
security significantly outweigh the overhead, with the number of iterations
offering useful flexibility.


To showcase our techniques, we apply them to lattice-based signatures.
Specifically, we introduce a new random-probing composable gadget for sampling
small noise, a key component in various post-quantum algorithms. To assess
security in this context, we generalize the random probing security model to
address auxiliary inputs and public outputs. We apply our findings to Raccoon, a
masking-friendly signature scheme originally designed for standard probing
security. We prove the secure composition of our new gadgets for key generation
and signature computation, and show that our masking scheme achieves a superior
security-performance tradeoff compared to previous approaches based on random
probing expansion. To our knowledge, this is the first fully secure
instantiation of a post-quantum algorithm in the random probing model.
