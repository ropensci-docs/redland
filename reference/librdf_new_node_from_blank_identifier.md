# Constructor - create a new blank node librdf_node object from a blank node identifier.

Constructor - create a new blank node librdf_node object from a blank
node identifier.

## Usage

``` r
librdf_new_node_from_blank_identifier ( world,
  inStrOrNull )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- inStrOrNull:

  UTF-8 encoded blank node identifier or NULL ("character")

## Value

\_p_librdf_node_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
