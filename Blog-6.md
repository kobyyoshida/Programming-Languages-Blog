Unison

What is it?

Unison is a programming language based on content-addressed code. This means we define function by a hash instead of by naming. Every function, variable and operator is represented by a hash, making it a very uniform programming language. Unison is simple, flexible and in some cases optimal. 

Benefits

No builds: Once we compile and a function is saved as a hash, it never has to be compiled again, we just refer to the hash. This is lighter on memory and overall computational cost.

Easy Renames

Durable Storage: Basically, when you compile the hashes are saved into a database like data structure. Since they are saved efficiently, if we delete a code block, we can retrieve the deleted function based off the hash.

Eliminates Dependency Conflicts: Often times, when code has been updated there are dependency conflict due to naming conventions. Specifically, a function has been adjusted in an update, but a team of programmers with some programmers using the old version and some using the new version run into conflicts when a function has been updated. In Unison, this does not happen because hashes are always unique, and small differences in functions can be handled easily as two different hashes.


Link
https://www.youtube.com/watch?v=gCWtkvDQ2ZI