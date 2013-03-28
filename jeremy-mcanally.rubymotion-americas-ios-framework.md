# RubyMotion: AMERICA'S IOS FRAMEWORK

## by Jeremy McAnally

### Abstract

I was recently invited to take part in a hackathon at the White House, at which I built a ridiculously boss iPhone app using RubyMotion for the We The People petition site.  It consumes the soon-to-be-published We The People API and provides an attractive way to browse the various petitions on the site.  Very likely, it is the greatest iPhone application ever created.

Had I attempted to build the same app using Objective-C, I'm pretty sure that I wouldn't have gotten nearly as far in the one day timeframe I had before me.  RubyMotion was more comfortable for me and gave me a good set of tools to build things quickly.  Then again, even as an experienced Ruby developer, I hit some stumbling blocks with RubyMotion.  This talk is a quick walkthrough of basic RubyMotion usage, followed by 4 stumbling blocks that developers may hit and how to overcome them:

* **Gems are cray.**  Gems require specific adaptation to be used in RubyMotion due to runtime restrictions.
* **Cocoa is quirky.**  I've done a good bit of Objective-C development, but the other Ruby developers I had help me with things found its patterns a little odd.
* **Building a UI is awkward.**  UIs are, by their nature, visual, so building one out with code can be awkward.
* **Errors can be obtuse.**  Tracing back errors can be a pain, especially if they're deep in the stack.

I'll talk about each pain point and a few solutions to each.  The idea of this talk is to reduce friction for Ruby developers who want to start using RubyMotion, but who will very likely encounter these same issues with little to no help on them as it is.

### Additional Notes

I am awesome.  Actually, that's rather false, but I really like Boston a lot.  That counts for something, right?

## Social ##

* [http://jeremymcanally.com](My website)
* [http://twitter.com/jm](@jm)
* [https://github.com/jm](GitHub)
