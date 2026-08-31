# Constructor - create a new resource librdf_node object with a given URI and local name.

Constructor - create a new resource librdf_node object with a given URI
and local name.

## Usage

``` r
librdf_new_node_from_uri_local_name ( world,
  uri,
  local_name )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- uri:

  librdf_uri object ("\_p_librdf_uri_s")

- local_name:

  local name to append to URI ("character")

## Value

\_p_librdf_node_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
