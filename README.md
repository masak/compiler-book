So, I'm writing a compiler book. Inspiration comes from [this HN comment](http://news.ycombinator.com/item?id=3840545).
Kudos also to [Matthew Walton](http://twitter.com/#!/MaW/status/191172939301920768)
for thinking it'd be a good idea. ☺

These plans will most likely converge with bootstrapping
<del>[007](https://github.com/masak/007)</del> [Alma](https://github.com/masak/007/issues/277), and successively building out the language
and the compiler can be interwoven with explaining and building optimizations.
The different compiler steps can even be used as realistic benchmarking
targets.

The plan that falls out of that idea is something like this:

* Variables and assignments
    * Constant folding
    * Constant propagation
    * Common subexpression elimination
    * Dead code elimination
* Integers and strings
* Control flow: if, while, and for
    * Basic blocks
    * SSA
    * Live variables analysis
    * Define-use chain analysis
    * Strength reduction
* Subroutines
    * Inlining
    * Closures
    * Escape analysis
    * Lowering to local variables
    * Built-in functions
* Register allocation
    * A naive allocator
    * Graph coloring
    * A linear allocator
* Modules
* Operators
    * Precedence and associativity
    * Built-in operators
    * Parsing user-defined operators
* Classes and objects
    * Dynamic dispatch
    * Lowering to primitives
    * Scalar replacement
    * First-class subroutines
    * Garbage collection
    * Built-in classes
* Meta-object protocol
    * `Object` and `Type`
    * Bootstrapping everything
* Type declarations
    * Typed variables and parameters
    * Type inference
    * Interfaces
    * Generic types
* Macros
* JIT
* ...
* IDE errors and warnings (using the IntelliJ stack)

## Material

I expect to delve deeply into [the Dragon book](http://www.amazon.com/Compilers-Principles-Techniques-Tools-Edition/dp/0321486811),
[SICP](http://www.amazon.com/Structure-Interpretation-Computer-Programs-Edition/dp/0070004846),
and [Modern Compiler Design](http://www.amazon.com/Modern-Compiler-Design-D-Grune/dp/0471976970) in
order to learn more of the theory and practice of writing compilers. It'll be both a learning
experience and a teaching experience. ☺

vendethiel suggested I have a look at [this set of AST-based compiler optimizations](https://github.com/estools/esmangle/tree/master/lib/pass). Looks very cool. Apparently there's a [tool](https://github.com/estools/esmangle/tree/master/test/compare) to see exactly what an optimization did.

[This post](https://github.com/jozefg/pcf/blob/master/explanation.md) about compiling a small example language to C is just incredibly clear and inspiring.

Here's a nice [collection of links](https://stackoverflow.com/questions/1669/learning-to-write-a-compiler).

I found [T3X](https://www.t3x.org/t3x/), a nice small self-hosting language/compiler.
