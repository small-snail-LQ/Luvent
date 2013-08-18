Luvent: A Simple Event Library for Lua
======================================

**Luvent is in early development and not recommended for any
  production software.  The API is subject to change and break
  compatibility without warning.**

Luvent is a library for [Lua][], written entirely in Lua, which helps
support [event-driven programming][EDP].  Luvent lets you create
events, which are objects with any number of associated functions.
Whenever you trigger an event the library will execute all functions
attached to that event.  You may trigger an event multiple times and
can provide different arguments that event’s functions each time.


Requirements
------------

Luvent requires one of the following Lua implementations:

* Lua 5.1.5
* Lua 5.2.2
* [LuaJIT][] 2.0.2

These are the versions we use to test Luvent.  It should work with
later versions of each, and possibly older versions as well.

### Optional ###

The following programs are not necessary in order to use Luvent but
you will need them to run the unit tests, generate API documentation,
and so on.

* [LuaDoc][]
* [busted][]


Documentation
-------------

Running the command `make docs` will populate the `docs/` directory
with HTML documents that describe Luvent’s API.


Acknowledgments
---------------

[EventLib][] by Elijah Frederickson is the major inspiration for the
design and implementation of Luvent.  The Luvent API also owes a debt
of ideas and names to [Node.js][] by Ryan Dahl et al.


License
-------

[The MIT License](http://opensource.org/licenses/MIT)

Copyright 2013 Eric James Michael Ritz



[Lua]: http://lua.org/
[EDP]: http://en.wikipedia.org/wiki/Event-driven_programming
[EventLib]: https://github.com/mlnlover11/EventLib
[Node.js]: http://nodejs.org/
[LuaJIT]: http://luajit.org/
[LuaDoc]: http://keplerproject.github.io/luadoc/
[busted]: http://olivinelabs.com/busted/