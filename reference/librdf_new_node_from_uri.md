# Constructor - create a new resource librdf_node object with a given URI.

Constructor - create a new resource librdf_node object with a given URI.

## Usage

``` r
librdf_new_node_from_uri ( world,
  uri )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- uri:

  librdf_uri object ("\_p_librdf_uri_s")

## Value

\_p_librdf_node_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
