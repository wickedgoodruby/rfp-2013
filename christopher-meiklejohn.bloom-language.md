# Bloom: A language for disorderly distributed programming #

## by Christopher Meiklejohn ##

### Abstract ###

Traditional programming languages use a model of computation where
individual instructions are executed in order.  However, when building
distributed systems this model fails to match the reality of how your
application code is actually executed.  Bloom is a language which allows
programmers to build applications as a series of unordered statements
while also providing facilities for imposing a particular ordering of
events when necessary.

During this talk we will explore building applications in Bud, which is
a prototype of Bloom implemented as a domain specific language in Ruby.
We will discuss the concepts of logical monotonicity, disorderly
collections, the CALM principle which is the root of the Bloom language,
and how to use he Bloom language to identify critical sections of your
code where a coordiation library should be used to ensure consistency.

### Additional Notes ###

Christopher Meiklejohn is a Software Engineer with Basho Technologies, Inc.
where he focuses on building rich web applications for Riak using Erlang and
JavaScript. Before joining Basho, he worked at Swipely, a loyalty program
startup based in Providence where he maintained critical infrastructure
components written in Ruby. Christopher currently serves as one of the
maintainers of Rubygems.org.

Christopher speaks frequently at meetups about JavaScript and Rich Internet
Applications, co-organized DowncityJS, and has most recently spoken at Web
Unleashed '12 and Clojure/West '13.  Christopher is also a graduate student in
computer science at Brown University, in Providence RI.

## Social ##

* [http://twitter.com/cmeik](@cmeik)
* [https://github.com/cmeiklejohn](GitHub)
