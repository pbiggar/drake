- Declarative foreign function interface
  - allows for reimplementation
- Separated compilation and run-time phases
  - Type-based metaprogramming in the compilation phase
- Almost nothing built into the language
- infinite precision integers by default

- module-system:

  - let 3rd party modules feel as natural as 1st party
  - solve metaprogramming without resorting to monkey patching
  - allow each "compilation unit" (whatever that means) to use its own libs and naming, without damaging other
  - so a static module system

- type system:
  - separate the three uses of types:
    - code reuse (inheritence, mixins)
    - object "type" identification (partly inheritence)
    - type checking
  - only objects, no run-time types
  - interfaces can be defined, and used to statically and dynamically type-check
    - can be made fast using shapes/hidden-classes both statically and dynamically
    - very closely related to structural typing (I think)
  - related to the modules system
