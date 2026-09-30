# Return the properties pointing from the given resource.

Return the properties pointing from the given resource.

## Usage

``` r
librdf_model_get_arcs_out ( model,
  node )
```

## Arguments

- model:

  librdf_model object ("\_p_librdf_model_s")

- node:

  librdf_node resource node ("\_p_librdf_node_s")

## Value

\_p_librdf_iterator_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
