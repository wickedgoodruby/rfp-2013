# Have you ever...faked it?

## Harlow Ward

### Abstract

Whether working in Rails, Sinatra, or Ruby command-line applications most
projects will interact with data from outside sources. This could come in the
form of a Payment Gateway, Social Network, or a 3rd party CRM.

It is important to remove interactions with external services while running
tests. Removing external requests will help alleviate the following scenarios:

* Slow tests due to external HTTP requests.
* Hitting production APIs with test data.
* Developing against a web service that doesn't exist yet.

We'll discuss, and demonstrate the use of Mocking, Stubbing,
and creating Fake Services. These techniques will keep our test suites
running fast, and ensure we're always testing in isolation.

### Additional Notes

I'm a Ruby on Rails developer at [thoughtbot](http://www.thoughtbot.com), Co-author of
[Ruby Science](http://www.rubyscience.com), and Co-presenter of the
[TDD Intro Track](http://railsconf.com/2013/talks#talk-64) at RailsConf 2013.

This will be my first time giving this talk and I'm really excited about the topic.
I think its an important part of testing our applications, and I'm super enthusiastic
about the idea of sharing techniques with the community.

## Social

* [hward.com](http://www.hward.com)
* [@futuresanta](http://twitter.com/futuresanta)
* [GitHub](https://github.com/harlow)
