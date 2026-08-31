# Set the query-specified limit on results.

Set the query-specified limit on results.

## Usage

``` r
librdf_query_set_limit ( query,
  limit,
  .copy )
```

## Arguments

- query:

  librdf_query query object ("\_p_librdf_query")

- limit:

  the limit on results, \>=0 to set a limit, \<0 to have no limit
  ("integer")

- .copy:

  NA

## Value

integer

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
