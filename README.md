# Ranch

![Ranch OpenRiak Status](https://github.com/OpenRiak/ranch/actions/workflows/erlang.yml/badge.svg?branch=openriak-3.2)

Ranch is a socket acceptor pool for TCP protocols.

## Goals

Ranch aims to provide everything you need to accept TCP connections with
a *small* code base and *low latency* while being easy to use directly
as an application or to *embed* into your own.

Ranch provides a *modular* design, letting you choose which transport
and protocol are going to be used for a particular listener. Listeners
accept and manage connections on one port, and include facilities to
limit the number of *concurrent* connections. Connections are sorted
into *pools*, each pool having a different configurable limit.

Ranch also allows you to *upgrade* the acceptor pool without having
to close any of the currently opened sockets.

## Online documentation

- [User guide](https://ninenines.eu/docs/en/ranch/2.1/guide)
- [Function reference](https://ninenines.eu/docs/en/ranch/2.1/manual)

## Offline documentation

- While still online, run `make docs`
- User guide available in `doc/` in PDF and HTML formats
- Function reference man pages available in `doc/man3/` and `doc/man7/`
- Run `make install-docs` to install man pages on your system
- Full documentation in Asciidoc available in `doc/src/`
- Examples available in `examples/`

## Getting help

- [Issues tracker](https://github.com/ninenines/ranch/issues)
- [Commercial Support](https://ninenines.eu/services)
