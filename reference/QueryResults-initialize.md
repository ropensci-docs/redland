# Initialize the QueryResults object.

The QueryResults object is initialized with the librdf query result from
return value of `'Query.execute()'`.

## Usage

``` r
# S4 method for class 'QueryResults'
initialize(.Object, results)
```

## Arguments

- .Object:

  the QueryResults object.

- results:

  a librdf query result

## Value

the QueryResults object

## Details

A QueryResults object is returned by the `Query.executeQuery()` method,
so typically a user does not initialize a QueryResult object by calling
`new("QueryResult", ...)`
