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

I expect to delve deeply into [the Dragon book](http://www.amazon.com/Compilers-Principles-Techniques-Tools-Edition/dp/0321486811),
[SICP](http://www.amazon.com/Structure-Interpretation-Computer-Programs-Edition/dp/0070004846),
and [Modern Compiler Design](http://www.amazon.com/Modern-Compiler-Design-D-Grune/dp/0471976970) in
order to learn more of the theory and practice of writing compilers. It'll be both a learning
experience and a teaching experience. ☺

Oh, and the plan is to use Perl 6 as the implementation language throughout the
book. Partly because it's a pleasant langauge which will easily and succinctly
express the points of the text; partly because it'll give us parsing for free
through grammars. So we don't have to reinvent the wheel there. In fact, that's
part of the intended use of Perl 6 &mdash; as a sort of "language incubator".
