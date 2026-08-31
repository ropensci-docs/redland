# Constructor - create a new librdf_uri object from a URI string.

Constructor - create a new librdf_uri object from a URI string.

## Usage

``` r
librdf_new_uri ( world,
  string )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- string:

  URI in string form ("character")

## Value

\_p_librdf_uri_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
