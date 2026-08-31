# Initialize a Parser object.

A Parser object is initialized for a specific RDF serialization.

## Usage

``` r
# S4 method for class 'Parser'
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

  the Parser object

- world:

  a World object

- name:

  name of the parser factory to use

- mimeType:

  a mime type of the syntax of the model

- typeUri:

  a URI for the syntax of the model

## Value

the Parser object

## Details

The serialization format that are supported by
