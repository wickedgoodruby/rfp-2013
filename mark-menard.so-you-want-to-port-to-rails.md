# So, You Want to Port to Rails #

## by Mark Menard ##

### Abstract ###

You have a legacy app that you wish was running on Rails. Get some insight from a port of a seven year old application written in Java and Groovy using Struts 2, JPA and a bunch of other Java frameworks. Learn the strategies we used to successfully port core business logic while maintaining correctness. How we leveraged JRuby to enable an incremental approach. How we ported tests while maintaining the same semantics. How we automated translation of code from Java and Groovy to Ruby. How we were able to make the system more easily modular and break it into services. Where we tripped up, and caused ourselves problems. Learn from our mistakes so you don't have to repeat them. And finally why would you EVER do this?

### Additional Notes ###

Myself and my team have been working with JRuby in production since August 12, 2008 starting with Rails 2.1. We have gained a lot of experience working with JRuby and integrating with Java libraries, and running Rails in conjunction with other Java web frameworks. Recently our client asked us to port the Java and Groovy portion of their application to Rails.

A few years ago I undertook an attempt at porting the services layer of this application to Ruby and Active Record and stopped because it was a flawed approach. The lessons learned from that effort fed into the current port and have helped it succeed.

I attended the Voices that Matter Ruby conference ages ago. It would be awesome to come back and reconnect with 

My speaker bio:

Mark Menard is the founder of Enable Labs, a boutique consulting firm, in Troy, NY, specializing in product develoment, business productity and problem solving. Mark recently did the Intro to Ruby and Rails at LosAngeles Ruby Conf, and has spoken on Ruby at several events including BarCamp Albany and CodeCamp Albany. He has also spoken on Software Patents at TEDxAlbany in 2010. Mark frequently presents on Ruby issues at the TechValley Ruby Brigade; and does training sessions covering Ruby, Rails, refactoring, test/behavior driven development, and other software development topics.

Mark used to be a Java developer and caught the dynamic language bug when he started coding in Groovy and then discovered Ruby. Since then he has added iOS development using Objective-C, Ruby's twin separated at birth.

## Social ##

* [http://enablelabs.com](Business Site)
* [http://twitter.com/mark_menard](Twitter)
* [https://github.com/MarkMenard](GitHub)
