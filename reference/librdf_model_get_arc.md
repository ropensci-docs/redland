# Return one arc (predicate) of an arc in an RDF graph given source (subject) and target (object).

Return one arc (predicate) of an arc in an RDF graph given source
(subject) and target (object).

## Usage

``` r
librdf_model_get_arc ( model,
  source,
  target )
```

## Arguments

- model:

  librdf_model object ("\_p_librdf_model_s")

- source:

  librdf_node source ("\_p_librdf_node_s")

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
