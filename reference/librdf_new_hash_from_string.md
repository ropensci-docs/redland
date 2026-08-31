# Constructor - create a new librdf_hash object from a string.

Constructor - create a new librdf_hash object from a string.

## Usage

``` r
librdf_new_hash_from_string ( world,
  name,
  string )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- name:

  hash name ("character")

- string:

  hash encoded as a string ("character")

## Value

\_p_librdf_hash_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
