# Constructor - create a new librdf_query object.

Constructor - create a new librdf_query object.

## Usage

``` r
librdf_new_query ( world,
  name,
  uri,
  query_string,
  base_uri )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- name:

  the name identifying the query language ("character")

- uri:

  the URI identifying the query language (or NULL) ("\_p_librdf_uri_s")

- query_string:

  the query string ("character")

- base_uri:

  the base URI of the query string (or NULL) ("\_p_librdf_uri_s")

## Value

\_p_librdf_query

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
