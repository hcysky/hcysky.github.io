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
- Example: arithmetic multiplication in GF(2^8)

{02}\*{87} mod {11B} = {0000 0010}\*{1000 0111} mod {1 0001 1011}
=x \* (x^7+x^2+x+1) mod (x^8+x^4+x^3+x+1)
=(x^8+x^3+x^2+x) mod (x^8+x^4+x^3+x+1)
=x^4+x^2+1={0001 0101}


- Polynomial arithmetic operations:
Let f(x)=x^3+x^2, g(x)=x^2+x+1
Then,
(Addition) f(x)+g(x)=x^3+x+1
(Multiplication) f(x) \* g(x) = x^5+x^2

- Polynomial division

f(x) = q(x) \* g(x) + r(x), where q(x) is quotient, g(x) is divisor, r(x) is remainder.
Let f(x)= x^3+x+1, g(x)=x+1
(Division) r(x)=reminder=f(x) mod g(x) = 1, q(x)=x^2+x (quotient), g(x)=x+1 (modular polynomial.


Reference
====

- [ ] [AES Arithmetic](https://uomustansiriyah.edu.iq/media/lectures/5/5_2020_12_28!10_55_23_AM.pdf)
