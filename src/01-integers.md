# Integers

We start by defining a simple language with integers, some operations, and printing.

    n = 5;
    sq = n * n;
    say(sq);

The language has two types of statement: variable assignment and printing.

It also has expressions, which can contain the following things:

* Terms: variables, integer literals
* Operators: +, -, *, % (all four infix, the first two also prefix)

XXX Show first a manual recdescent approach

XXX Then maybe how to get a lot closer to EBNF with a macro approach

XXX Talk about generating an AST for this

XXX Optimizations -- but since the language is so simple, we can just eval everything at compile time
