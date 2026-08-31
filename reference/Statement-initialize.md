# Construct a Statement object.

Construct a Statement object.

## Usage

``` r
# S4 method for class 'Statement'
initialize(
  .Object,
  world,
  subject,
  predicate,
  object,
  subjectType = as.character(NA),
  objectType = as.character(NA),
  datatype_uri = as.character(NA),
  language = as.character(NA)
)
```

## Arguments

- .Object:

  the Statement object

- world:

  a World object

- subject:

  a Node object

- predicate:

  a Node object

- object:

  a Node object

- subjectType:

  the Node type of the subject, i.e. "blank", "uri"

- objectType:

  the Node type of the object, i.e. "blank", "uri", "literal"

- datatype_uri:

  the datatype URI to associate with a object literal value

- language:

  a character value specifying the RDF language tag for an object
  literal value (excluding the "@" symbol), i.e. "fr"

## Value

the Statement object
