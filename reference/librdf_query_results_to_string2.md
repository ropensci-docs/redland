# Turn a query results into a string.

Turn a query results into a string.

## Usage

``` r
librdf_query_results_to_string2 ( query_results,
  name,
  mime_type,
  format_uri,
  base_uri )
```

## Arguments

- query_results:

  librdf_query_results object ("\_p_librdf_query_results")

- name:

  format name ("character")

- mime_type:

  format mime type (or NULL) ("character")

- format_uri:

  URI of syntax to format to (or NULL) ("\_p_librdf_uri_s")

- base_uri:

  Base URI of output formatted syntax (or NULL) ("\_p_librdf_uri_s")

## Value

character

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
