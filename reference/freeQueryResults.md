# Free memory used by a librdf query results

After this method is called, the QueryResults object is no longer usable
and should be deleted with `"rm(query)"`.

## Usage

``` r
freeQueryResults(.Object)

# S4 method for class 'QueryResults'
freeQueryResults(.Object)
```

## Arguments

- .Object:

  a QueryResults object
