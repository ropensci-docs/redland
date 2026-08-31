# Search the model for matching statements in a given context.

Search the model for matching statements in a given context.

## Usage

``` r
librdf_model_find_statements_in_context ( model,
  statement,
  inNodeOrNull )
```

## Arguments

- model:

  librdf_model object ("\_p_librdf_model_s")

- statement:

  librdf_statement partial statement to find ("\_p_librdf_statement_s")

- inNodeOrNull:

  context librdf_node (or NULL) ("\_p_librdf_node_s")

## Value

\_p_librdf_stream_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
