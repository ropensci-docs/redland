# Execute a query against the model.

Execute a query against the model.

## Usage

``` r
librdf_model_query_execute ( model,
  query )
```

## Arguments

- model:

  librdf_model object ("\_p_librdf_model_s")

- query:

  librdf_query object ("\_p_librdf_query")

## Value

\_p_librdf_query_results

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
