Invariants

An invariant is a value that remains the same throughout a computation. An invariant can be used as a problem solving technique. Typically in class, we start with a combination of a's and b's and try to rearrange them into normal form, where they are organized into a's first, followed by b's. 

Invariants can be:
    length of equation
    number of a's
    number of b's
    number of a's + number of b's
    number of a's = number of b's
    any function that returns the same value before and after computation

A function is an invariant for an ARS if:
a -> b => P(a) = P(b)

Invariants can be used to prove termination, as well as find errors. For example, if a value is supposed to return NULL for every possible input, but we find a value of 0 for an unexpected input value, we have found a flaw in our code that needs to be fixed. 

Example

Given this set of rewrite rules, find the normal form of the string XaaaYbbZ by using an invariant.

aYb -> a$bY
a$b -> $bca
ac -> ca
X$b -> X
Xc -> cX
YZ -> Z
aZ -> Z
XZ ->

After reducing the string by hand, we can try different inputs in the form XAYBZ where A is any number of a's and B is any number of b's. We will find that the normal form of any string inputted in this format will be a number of c's as follows:

(number of a's * the number of b's) = number of c's

