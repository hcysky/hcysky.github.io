---
title: 'AES Arithmetic Operation'
date: 2024-09-23
permalink: /_posts/2024/09/aes-arithmetic-operation/
tags:
  - AES
  - Encryption & Decryption
  - Security
---

This is a blog post about AES arithmetic operation.

Definition
======

- Finite Field: a field with finite number of elements, also known as Galois Field.
- GF(p^n): the number of elements is always a power of a prime number.
- GF(p): the set of integer {0,1,...,p-1} with arithmetic operations modulo prime p.
- AES uses arithmetic in the finite field GF(2^8) with irreducible (prime) polynomial m(x)=x^8+x^4+x^3+x+1, which is {1 0001 1011} in binary or {11B} in hex.
- 





Reference
====

- [ ] [AES Arithmetic](https://uomustansiriyah.edu.iq/media/lectures/5/5_2020_12_28!10_55_23_AM.pdf)
