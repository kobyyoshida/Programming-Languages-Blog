Monoids vs Monads in Haskell


Monoids 

A monoid is a type with some rule for combining two same-type elements into one object of the same type. It is the single most natural operation for combining values. For example, additon or multiplication.

Division is not considered a monoid because the order of elements matters. If we ran a division function recursively on a list of many integers, the order in which we ran the division would determine a different result. 

Example

Given two lists, [10,20] and [50,100], we can join these together with a monoid to get [10,20,50,100].

Monads

A monad is a method to organize computations into terms of sequences of values. In other words, monads are a pattern for chaining together operations. This allows programmers to break down larger computations into individual steps. Monads are central to understanding input and output in Haskell. Monads allow programmers to separate combinations of computations, and isolate computations from the main body of a program.


Monoids vs Monads

Technically, a monad is a monoid. However, there are differences when they are put to use. Typically, a monoid is the smallest operation of combination of elements. A monad is a specific type of monoid where we are breaking down a computation into each step of said computation. 

Functors

A functor is a constant that transforms each element of a list. For example, if we multiplied each integer in a list by 3, or added an x to the end of every string in a list. Functors are relevant to monads and monoids because every monad is using some sort of functor to complete its task.