# Construct a Serializer object.

Construct a Serializer object.

## Usage

``` r
# S4 method for class 'Serializer'
initialize(
  .Object,
  world,
  name = "rdfxml",
  mimeType = "application/rdf+xml",
  typeUri = as.character(NA)
)
```

## Arguments

- .Object:

  the Serializer object

- world:

  a World object

- name:

  name of a previously created serializer factory to use

- mimeType:

  a mime type of the syntax of the model

- typeUri:

  a URI for the syntax of the model

## Value

the Serializer object
