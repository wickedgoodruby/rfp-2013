# Zen and the Art of Chef Metaprogramming #

## by Simeon Simeonov ##

### Abstract ###

[Chef](http://www.opscode.com/chef/) has become the de facto standard for deploying complex systems to the cloud. Although built in Ruby, Chef can sometimes be frustratingly un-Ruby-like. While SysAdmins may not care and hack their way through the mess, those practicing the Ruby Way make the mess go away. 

**chef + elegant\_metaprogramming == deployment.headaches.lower_by(:much).tap { win! }**

In this talk you'll learn how to get the most out of your & existing community cookbooks and resource providers though techniques such as:

- Escaping Chef's `#method_missing` insanity.

- Extending the Chef DSL to handle common usage patterns with less code.

- Subclassing lightweight resource providers (LWRPs) using a new cookbook from [Swoop](http://swoop.com).

- Dynamically-generating ChefSpec/Rspec matchers so that you spend less time debugging and more time deploying.

This talk is for Rubyists who care about seamless continuous deployment to the cloud and think that sysadmin work is software engineering gone (very) wrong. It is also a great topic for anyone interested in practical Ruby metaprogramming.

### Additional Notes ###

The talk is never before released content that shares how Swoop's engineering team approached Chef not as a SysAdmin tool but a pattern-based software deployment framework. Chef's abstractions did not match the reality of how we saw our system and so we used the power of Ruby to allow our intent to be expressed in our cookbooks. By the time of the conference we should be ready to open-source a cookbook that includes majik-class utilities such as subclassing Chef's LWRPs (see https://gist.github.com/ssimeonov/5811992 for an example).

I am the founder & CTO of Swoop, a search advertising platform. I built my first Rails app back in 2005 and Ruby has been my main programming language for the past several years. A long time ago, I was the chief architect of the team that built the first Web application server (ColdFusion). We ran some of the largest sites on the Net: from Priceline to MySpace. In between I've started half-a-dozen companies and invested in many more. 

## Social ##

* [http://swoop.com](Swoop)
* [http://blog.simeonov.com](blog)
* [http://twitter.com/simeons](@simeons)
* [https://github.com/ssimeonov](GitHub)
* [https://linkedin.com/in/simeons](LinkedIn)
