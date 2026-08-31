# Get the query result limit

Get the query result limit

## Usage

``` r
getQueryResultLimit(.Object)

# S4 method for class 'Query'
getQueryResultLimit(.Object)
```

## Arguments

- .Object:

  a Query object

## Value

the query result limit. If a limit is set then the value will be \>= 0.
If the value is \< 0, no limit is set
