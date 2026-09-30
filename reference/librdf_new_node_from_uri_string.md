# Constructor - create a new librdf_node object from a URI string.

Constructor - create a new librdf_node object from a URI string.

## Usage

``` r
librdf_new_node_from_uri_string ( world,
  string )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- string:

  string representing a URI ("character")

## Value

\_p_librdf_node_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
