# Object Pools

A rudimentary object pool library for Julia. 

An object pool is a threadsafe container of pre-initialized objects, typically
objects that are somewhat expensive to initialize. The idea here is that,
rather than repeatedly initializing and destroying these expensive objects,
objects can be pulled from the pool and returned to the pool as needed, recycling
them in a threadsafe fashion.
