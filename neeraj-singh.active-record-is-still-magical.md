# ActiveRecord is still magical #

## Neeraj Singh ##

### Abstract ###

ActiveRecord is complex code and because of complexity it has edge
cases. In fact lots of edge cases.
We will take a look at a number of ActiveRecord features to see how it works and how to deal with some of
the edge cases.

We will see how default_scope works. And why method "unscoped" removes default_scope from models but not from associations.

Do you know the difference between CollectionProxy and Relation ? Do you
know why in a has_many through case "@physician.patients.create!" would
work but "@physician.patients.where(active: true).create! would silently
fail without creating the association record ?

We will discuss why while patching Active Record you should run your tests against all three databases.

Guess which of these two obey :destroy option: @customer.orders.delete(@order) or @customer.orders.destroy(@order) .

In Rails 3 when where conditions are merged then the last where
condition wins. In Rails 4 all the where conditions are 'And'ed. But not
defautl_scope. We will see how and why.

Will also discuss implementation detail of features like inverse_of, autosave and callbacks.

### Additional Notes ###

Last few months I have been fixing Active Record issues and in the
process have learned a lot about inner workings of Active Record. In this talk I will share some of
the things I learned.

## Social ##

* [BigBinary](http://bigbinary.com/neeraj)
* [http://twitter.com/neerajdotname](http://twitter.com/neerajdotname)
* [https://github.com/neerajdotname](http://github.com/neerajdotname)
