# Get one binding value for a given name in the current result.

Get one binding value for a given name in the current result.

## Usage

``` r
librdf_query_results_get_binding_value_by_name ( query_results,
  name )
```

## Arguments

- query_results:

  librdf_query_results query results ("\_p_librdf_query_results")

- name:

  variable name ("character")

## Value

\_p_librdf_node_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
