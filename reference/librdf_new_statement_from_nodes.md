# Constructor - create a new librdf_statement from existing librdf_node objects.

Constructor - create a new librdf_statement from existing librdf_node
objects.

## Usage

``` r
librdf_new_statement_from_nodes ( world,
  subject,
  predicate,
  object )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- subject:

  librdf_node ("\_p_librdf_node_s")

- predicate:

  librdf_node ("\_p_librdf_node_s")

- object:

  librdf_node ("\_p_librdf_node_s")

## Value

\_p_librdf_statement_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
