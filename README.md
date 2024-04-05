# front-end-kaleidoscope

A little compiler for a non-trivial language built for the Programming Languages and Compilers course @ UniMORE.

<br>

The _test_ directory contains...
- floor &rarr; rounds down a number to the closest integer <= to that number (whole or fractional)
- rand  &rarr; generate and print 10 pseudorandom numbers
- fibonacci &rarr; calculate the n-th Fibonacci number
- sqrt  &rarr; calculate the (approximate) square root of an arbitrary number
- eqn2  &rarr; calculate the solutions of a quadratic equation, given the coefficients a,b and c
- sqrt2 &rarr; like sqrt but uses the logical operator 'or'
- sqrt3 &rarr; like sqrt but uses the logical operators 'and' and 'not'

<hr>

### Requirements

- [![LLVM](https://img.shields.io/badge/LLVM-17.0.6-blue)](https://releases.llvm.org/)
- [![Bison](https://img.shields.io/badge/Bison-3.8.2-red)](https://www.gnu.org/software/bison/bison.html)
- [![Flex](https://img.shields.io/badge/Flex-2.6.4-green)](https://gothub.frontendfriendly.xyz/westes/flex/blob/master/README.md)

<hr>

### References
- https://llvm.org/docs/tutorial/MyFirstLanguageFrontend/index.html
