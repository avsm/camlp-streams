# The Stream and Genlex libraries for use with Camlp4 and Camlp5

The `camlpstreams` package provides two library modules:
- Stream: imperative streams, with in-place update and memoization of the latest element produced.
- Genlex: a small parameterized lexical analyzer producing streams of tokens from streams of characters.

The two modules are designed for use with [Camlp4](https://github.com/camlp4/camlp4/) and [Camlp5](https://github.com/camlp5/camlp5):
- The stream patterns and stream expressions of Camlp4/Camlp5 consume and produce data of type 'a Stream.t.
- The Genlex tokenizer can be used as a simple lexical analyzer for Camlp4/Camlp5-generated parsers.

The Stream module can also be used by hand-written recursive-descent parsers, but is not very convenient for this purpose.

The Stream and Genlex modules have been part of the OCaml standard library for a long time, and have been distributed as part of the core OCaml system. They will be removed from the OCaml standard library at some future point, but will be maintained and distributed separately in this `camlpstreams` package.
