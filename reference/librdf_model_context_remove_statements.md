# Remove statements from a model with the given context.

Remove statements from a model with the given context.

## Usage

``` r
librdf_model_context_remove_statements ( model,
  context,
  .copy )
```

## Arguments

- model:

  librdf_model object ("\_p_librdf_model_s")

- context:

  librdf_node context ("\_p_librdf_node_s")

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
