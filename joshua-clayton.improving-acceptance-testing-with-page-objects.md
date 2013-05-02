# Improving Acceptance Testing with Page Objects #

## by Josh Clayton ##

### Abstract ###

While following red/green/refactor in application code is great, developers
often forget tests are code too and need to be refactored as such. Page
Objects provide a layer of abstraction throughout tests which simplify
interaction through well-named methods and good object-orientation; this
pattern allows developers to manage dependencies, selectors, and leverage
RSpec's matcher syntax to write clean, focused tests which encapsulate DOM
interaction and page concepts concisely. This talk will cover the progression
of existing code bases to use Page Objects, Page Objects' benefits and practical
applications, and why Page Objects will improve your acceptance tests.

### Additional Notes ###

I wrote a brief introduction on Page Objects within the context of a Rails
application recently [on the thoughtbot
blog](http://robots.thoughtbot.com/post/35776432958/better-acceptance-tests-with-page-objects).

In this talk, I will briefly discuss how Cucumber and Gherkin were used "back
in the day" to write acceptance tests and how we have been migrating towards
more abstract tests with RSpec and Capybara. With this foundation laid, I will
introduce Page Objects and their benefits, how I discovered them through a
progression of refactoring my tests, how to refactor existing tests using Page
Objects, and patterns that emerged after migrating test suites to use this
pattern. Finally, I will cover caveats, tricks to using Page Objects
effectively, and when to avoid using Page Objects.

## Social ##

* [http://joshuaclayton.me](http://joshuaclayton.me)
* [@joshuaclayton](http://twitter.com/joshuaclayton)
* [GitHub](https://github.com/joshuaclayton)
