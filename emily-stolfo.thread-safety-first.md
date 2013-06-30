# Thread Safety First #

## by Emily Stolfo ##

### Abstract ###

We rubyists historically haven’t been in the habit of thinking about concurrency but the reality is that our thread-unsafe code often works by sheer luck.  There are different implementations of Ruby with their own semantics that can unearth challenging and unexpected concurrency bugs in our code.  We have to become more accustomed to writing threadsafe code in order to anticipate these potential surprises, especially in light of the rise in popularity of JRuby.

I will discuss approaches to writing threadsafe code in this talk, with a specific focus on performance considerations and testing.  I'll start by explaining some basic concurrency concepts, describe methods for handling shared mutable data, and touch on the subtleties of concurrency primitives (Queue, ConditionVariable, Mutex).  Hair-raising, real-world bugs will be used throughout the presentation to illustrate specific concurrency issues and techniques for solving them.

### Additional Notes ###

Jose Valim said in his keynote on concurrency at RubyKaigi 2013 that the Ruby community needs _education_ on the subject in addition to well-defined semantics, a thread-safe standard library, and high level abstractions.  This talk is intended to share some things I’ve learned about concurrency in Ruby using my experience in maintaining a driver to a database as an example.
 
At the beginning of this year, a user on JRuby brought a few concurrency concerns to the mongodb Ruby team’s attention.  After much work and thought, our code is threadsafe and we have a much deeper understanding of how threads work in MRI/YARV and JRuby and how to write threadsafe code.  The python driver had some of the same issues and our teams collaborated to improve both drivers.  Jesse Davis wrote a great [blog post](http://emptysqua.re/blog/wasps-nest-read-copy-update-python/) on the solution:  

A rough outline of the topics I will discuss:

* Main Example used throughout: Ruby driver to MongoDB.  We support MRI (YARV) and JRuby.  Important point: JRuby uses native threads and not green threads so bugs were unearthed by using JRuby.

#### Intro:

* Ruby has different implementations with their own semantics.  
* Our code sometimes works by accident.
* GVL, green threads, native threads
* JRuby threads usually map to native threads, not green threads.

#### Basic concurrency concepts
* Shared data. Examples..
* Native threads versus green threads and their implications
* Atomicity

#### Considerations when writing threadsafe code
* Avoid sharing data across threads
* Identify shared data and isolate it
* Identify shared, MUTABLE data and see if you can avoid this dependency
* Synchronize the mutation of shared mutable data. 
    + Mutex, Queue, ConditionVariable 
    + Considerations when synchronizing
* Testing
	
#### How to use concurrency primitives
* ConditionVariable
* Mutex

#### Conclusion
* Get in the habit of thinking about shared mutable data and atomicity
* Test against JRuby
* Get to know the concurrency primitives
* Use the Ruby driver!  It’s threadsafe!!

## Social ##

* [@EmStolfo](http://twitter.com/EmStolfo)
* [estolfo's github](https://github.com/estolfo)