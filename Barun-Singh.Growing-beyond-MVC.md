# Growing beyond MVC

## by Barun Singh

### Abstract ###

Rails comes pre-packaged with an MVC architecture, and Rails developers often debate how best to structure their applications accordingly. A well-informed developer will usually start with a simple set of goals:

* Controllers should be simple and concise
* Classes should have a single responsibility
* Views should not contain any logic

Initially, for small applications, keeping things clean is pretty easy. Sure, you get a few small methods here and there that don't quite fit just right, or your models start doing just a tiny amount of work that maybe they shouldn't do, but you can handle it. But eventually, these minor compromises add up and you notice that your codebase is littered with all sorts of anti-patterns. 

* Complex callbacks that cause models to know far too much about each other
* Models have methods that contain no business logic, but only serve to be referenced by views
* Helper methods that get put into dozens of modules that made sense once, but now seem a bit arbitrary
* Models that are hundreds of lines long 

In this talk, I'll be discussing ways to augment the Model-View-Controller pattern to avoid these anti-patterns, even as your application grows. Specifically, I will discuss:

* Presenters as a better object-oriented alternative to helper methods and cluttered models
* Service Objects as a way to extract particular aspects of model logic into separate objects that encapsulate desired behavior
* Builders as a way to extract out create callbacks that interact with multiple models

We'll discuss how these concepts relate to those in other frameworks. Specifically, I'll describe parallels with Backbone.js, a common front-end companion for Rails apps.

At WegoWise, we've gone through all of these iterations and my talk will be based on the experiences our team has had in growing our application to one that has hundreds of classes, but is still easily refactored, tested, and understood by new developers.

## Social ##

* [http://barunsingh.com](barunsingh.com)
* [https://github.com/barunio](GitHub)
