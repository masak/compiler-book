So, I'm writing a compiler book. Inspiration comes from [this HN comment](http://news.ycombinator.com/item?id=3840545).
Kudos also to [Matthew Walton](http://twitter.com/#!/MaW/status/191172939301920768)
for thinking it'd be a good idea. ☺

Here's a tentative table of contents, cribbed straight from the HN comment in
question, but hopefully evolvable into something more complete:

* SSA
* abstract interpretation
* compiling high level languages
* pointer analysis
* compiling dynamic dispatch
* garbage collection 
* closures

Other ideas, added later:

* various optimizations, such as loop optimizations, strength reduction, and data-flow optimizations
* register allocation

I expect to delve deeply into [the Dragon book](http://www.amazon.com/Compilers-Principles-Techniques-Tools-Edition/dp/0321486811),
[SICP](http://www.amazon.com/Structure-Interpretation-Computer-Programs-Edition/dp/0070004846),
and [Modern Compiler Design](http://www.amazon.com/Modern-Compiler-Design-D-Grune/dp/0471976970) in
order to learn more of the theory and practice of writing compilers. It'll be both a learning
experience and a teaching experience. ☺

My plan:

* Use nqp as the implementation language/compiler platform. It has Perl 6 grammars and is meant
  to be used to build higher-level languages.
* Build a language (called "Nugget") which is easy to read and explain. It has a small core and
  is easy to improve in various directions. It is powerful enough to self-host a parser easily.

Oh, here's another link, [full of compiler optimizations](https://news.ycombinator.com/item?id=6273085). Might be useful when I dig into the literature.

vendethiel suggested I have a look at [this set of AST-based compiler optimizations](https://github.com/estools/esmangle/tree/master/lib/pass). Looks very cool. Apparently there's a [tool](https://github.com/estools/esmangle/tree/master/test/compare) to see exactly what an optimization did.
