# Strongly Typed, Shared Models for Services #

## by Tim Perkins ##

### Abstract ###

Whether we are breaking a big application down into services or designing a Service Oriented Architecture from the beginning, a key question is how the different services will communicate. Regardless of whether that communication is a web request, a message on a queue, or an RPC we must decide on the message formats.

In Ruby, it is easy to say that everything is Hash, and let the other end of the connection determine what to do with the contents. However with the inclusion of strong parameters in Rails 4, there is motivation to provide more structure for our web API requests. Other transport methods may also add requirements/constraints to minimize the size of the data transferred or to maximize the performance of serialization/deserialization.

In this talk, I will describe using the interface definition language Thrift (http://thrift.apache.org/) to define a model that is shared between a server and clients. I'll use the same Thrift-generated model to provide serialization for messages on queues and to drive the enforcement of strong parameter permissions through integration with Seahorse (https://github.com/awslabs/seahorse) models.

### Additional Notes ###

This talk has not been presented previously at any conference.

## Social ##

* [Yesware](http://www.yesware.com)
* [LinkedIn](http://linkedin.com/in/tjwperkins)
* [GitHub](https://github.com/tjwp-yesware)
