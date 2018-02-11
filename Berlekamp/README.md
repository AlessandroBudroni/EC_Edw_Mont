# Berlekamp

This is an implementation of the Berlekamp algorithm for factorising to factorize polynomials over finite fields.

Reference: Introduction to Finite Fields and their Applications, Lidl and Niederreiter, pag 130.

Author: Alessandro Budroni

EXAMPLE OF USAGE

```
> P<x> := PolynomialRing(GF(2));
> 
> p := x^127+x+1;
> 
> Berlekamp(p);
[
    <x^127 + x + 1, 1>
]

> q := x^127+x^5+1;
> Berlekamp(q);    
[
    <x^2 + x + 1, 1>,
    <x^3 + x^2 + 1, 1>,
    <x^5 + x^3 + 1, 1>,
    <x^46 + x^45 + x^44 + x^42 + x^40 + x^39 + x^38 + x^37 + x^36 + x^35 + x^34 + x^32 + x^30 + x^28 + x^27 + x^22 + x^20 + x^18 + x^17 + x^15 + x^14 + x^12 + x^8 + x^7 + x^5 + x + 1, 1>,
    <x^71 + x^70 + x^69 + x^66 + x^65 + x^64 + x^59 + x^58 + x^57 + x^55 + x^50 + x^49 + x^47 + x^45 + x^42 + x^40 + x^39 + x^38 + x^36 + x^34 + x^33 + x^32 + x^30 + x^29 + x^28 + x^25 + x^24 + x^22 + x^21 + 
        x^19 + x^16 + x^15 + x^14 + x^12 + x^11 + x^10 + x^9 + x^8 + x^5 + x^4 + x^3 + x^2 + 1, 1>
]

```
