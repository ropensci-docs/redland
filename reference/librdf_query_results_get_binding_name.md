# Get binding name for the current result.

Get binding name for the current result.

## Usage

``` r
librdf_query_results_get_binding_name ( query_results,
  offset )
```

## Arguments

- query_results:

  librdf_query_results query results ("\_p_librdf_query_results")

- offset:

  offset of binding name into array of known names ("integer")

## Value

character

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
