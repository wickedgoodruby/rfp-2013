# Supercharging ActiveRecord with PostgreSQL #

## by Dan McClain ##

### Abstract ###

You've been able to serialize Ruby objects with ActiveRecord in the past, but the database
treats serialized objects as text. PostgreSQL has support for advanced
data types, like arrays, hashes and ranges, natively, allowing the
database to do the heavy work for you. You can query a table for records that contain an
array with a specific element. You can build a reservation system in
which the database makes sure that you don't double book a room. All
of which happens in the database, preventing you from retrieving extra
records and processing them in memory.

With Rails 4, ActiveRecord has been supercharged. The PostgreSQL adapter
has been extended to support arrays and hashes, and was rewritten
to make adding your own types easier than before. There are gems out
there that allow you to leverage these datatypes in Rails 3 as well.


### Additional Notes ###

I am the author of the postgre\_ext gem, which adds ActiveRecord and
Arel support for PostgreSQL datatypes, and contributed commits to Rails
4.0 that added PostgreSQL array support


## Social ##

* [http://danmcclain.net](http://danmcclain.net)
* [@_danmcclain](http://twitter.com/_danmcclain)
* [GitHub](https://github.com/danmcclain)
