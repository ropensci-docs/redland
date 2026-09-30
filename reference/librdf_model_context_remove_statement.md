# Remove a statement from a model in a context.

Remove a statement from a model in a context.

## Usage

``` r
librdf_model_context_remove_statement ( model,
  context,
  statement,
  .copy )
```

## Arguments

- model:

  librdf_model object ("\_p_librdf_model_s")

- context:

  librdf_node context ("\_p_librdf_node_s")

- statement:

  librdf_statement statement ("\_p_librdf_statement_s")

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
