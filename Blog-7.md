Hoare Logic

Hoare Logic is a system with a set of rules for determining the correctness of programs. The purpose of Hoare Logic is to reason compositionally about the correctness of programs. Hoare Logic combines two ideas: a method of documenting specifications of programs, and a method of proving programs are correct.

Hoare Triple

A Hoare Triple is the main component of Hoare Logic. A triple describes how execution changes the state of a computation. 

Format

{P}C{Q}

where P is a precondition, Q is a postcondition, and C is a command or operation.

Example

{X=0} X:= X+1 {X=1}

This is a simple but proper Hoare Triple because X:= X+1 is an operation that would transform the state of X from 0 to 1.