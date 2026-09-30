# Return one source (subject) of arc in an RDF graph given arc (predicate) and target (object).

Return one source (subject) of arc in an RDF graph given arc (predicate)
and target (object).

## Usage

``` r
librdf_model_get_source ( model,
  arc,
  target )
```

## Arguments

- model:

  librdf_model object ("\_p_librdf_model_s")

- arc:

  librdf_node arc ("\_p_librdf_node_s")

- target:

  librdf_node target ("\_p_librdf_node_s")

## Value

\_p_librdf_node_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
