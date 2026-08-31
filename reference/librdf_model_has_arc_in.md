# Check if a node has a given property pointing to it.

Check if a node has a given property pointing to it.

## Usage

``` r
librdf_model_has_arc_in ( model,
  node,
  property,
  .copy )
```

## Arguments

- model:

  librdf_model object ("\_p_librdf_model_s")

- node:

  librdf_node resource node ("\_p_librdf_node_s")

- property:

  librdf_node property node ("\_p_librdf_node_s")

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
