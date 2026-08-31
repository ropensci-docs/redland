# Return the targets (objects) of an arc in an RDF graph given source (subject) and arc (predicate).

Return the targets (objects) of an arc in an RDF graph given source
(subject) and arc (predicate).

## Usage

``` r
librdf_model_get_targets ( model,
  source,
  arc )
```

## Arguments

- model:

  librdf_model object ("\_p_librdf_model_s")

- source:

  librdf_node source ("\_p_librdf_node_s")

- arc:

  librdf_node arc ("\_p_librdf_node_s")

## Value

\_p_librdf_iterator_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
