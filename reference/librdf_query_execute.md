# Run the query on a model.

Run the query on a model.

## Usage

``` r
librdf_query_execute ( query,
  model )
```

## Arguments

- query:

  librdf_query object ("\_p_librdf_query")

- model:

  model to operate query on ("\_p_librdf_model_s")

## Value

\_p_librdf_query_results

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
