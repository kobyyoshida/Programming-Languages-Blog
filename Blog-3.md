Abstract Reduction Systems

An Abstract Reduction System (ARS) is a set of rules for reducing objects in any system.
ARSs have two qualities in order to prove a normal form. ARSs are one-step computations, and is a fundamental feature for any computing. 

Confluence:

Whenever x reduces to y and z, then y and z are joinable. This essentially means an object can be broken down in many different ways, but always comes out to the same outcome.
If an ARS is confluent, we have an algorithm that decides whether two elements are equivalent.

Terminating:

There is no infinite chain a0 -> a1 -> a2 -> ...
Termination can be proved by showing that any input can be reduced to a normal form.

Example:
abab

Rewrite Rules:
ab -> ba
ba -> ab

This ARS does not terminate. The string will continue switching the places of a and b forever.

If we replace the rewrite rule "ab -> ba" with another rewrite rule ab ->  we can make the ARS terminate. With this rule in place, we should always get a normal form of [].