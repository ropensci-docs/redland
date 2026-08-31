# Initialize the Query object.

Initialize the Query object.

## Usage

``` r
# S4 method for class 'Query'
initialize(
  .Object,
  world,
  querystring,
  base_uri = NULL,
  query_language = "sparql",
  query_uri = NULL
)
```

## Arguments

- .Object:

  the Query object

- world:

  a World object

- querystring:

  a query string for the language specified in 'query_language'

- base_uri:

  a URI to prepend to relative URI in the document

- query_language:

  the query language to execute the querystring with

- query_uri:

  a URI to prepend to terms in the query

## Value

the Query object
