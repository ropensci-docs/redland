# Add a stream of statements to the model.

Add a stream of statements to the model.

## Usage

``` r
librdf_model_add_statements ( model,
  statement_stream,
  .copy )
```

## Arguments

- model:

  model object ("\_p_librdf_model_s")

- statement_stream:

  stream of statements to use ("\_p_librdf_stream_s")

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
