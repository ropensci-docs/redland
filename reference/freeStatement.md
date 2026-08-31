# Free memory used by a librdf statement

Free memory used by a librdf statement

## Usage

``` r
freeStatement(.Object)

# S4 method for class 'Statement'
freeStatement(.Object)
```

## Arguments

- .Object:

  a Statement object

## Details

After this method is called, the Statement object is no longer usable
and should be deleted `"rm(statement)"` and a new object created. This
method frees all resources for the statement, as well as each node in
the statement.

## Examples

``` r
world <- new("World")
stmt <- new("Statement", world, subject="http://www.example.com/myevent",
                                predicate="http://example.com/occurredAt",
                                object="Tue Feb 17 14:05:13 PST 2015")
# At this point, some operations would be performed with the Statement.
# See '?redland' for a complete example.
# When the Statement object is no longer needed, the resources it had allocated can be freed.
freeStatement(stmt)                                
#> NULL
rm(stmt)
```
