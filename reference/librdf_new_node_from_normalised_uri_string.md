# Constructor - create a new librdf_node object from a UTF-8 encoded URI string normalised to a new base URI.

Constructor - create a new librdf_node object from a UTF-8 encoded URI
string normalised to a new base URI.

## Usage

``` r
librdf_new_node_from_normalised_uri_string ( world,
  uri_string,
  source_uri,
  base_uri )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- uri_string:

  UTF-8 encoded string representing a URI ("character")

- source_uri:

  source URI ("\_p_librdf_uri_s")

- base_uri:

  base URI ("\_p_librdf_uri_s")

## Value

\_p_librdf_node_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
