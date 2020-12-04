Invariants

An invariant is a value that remains the same throughout a computation. An invariant can be used as a problem solving technique. Typically, we start with a combination of a's and b's and try to rearrange them into normal form, where they are organized into a's first, followed by b's. 

Invariants are:
    length
    number of a's
    number of b's
    number of a's + number of b's
    number of a's = number of b's
    any function that returns the same value before and after computation

A function is an invariant for an ARS if:
a -> b => P(a) = P(b)

In class we talked about the tile problem, where we have an nxn square of squares, where n >= 2 and n % 2 == 0. n is considered an invariant because the value of n does not matter, as long as it is even and n>1.