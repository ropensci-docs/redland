# Constructor - create a new librdf_hash object from an array of strings.

Constructor - create a new librdf_hash object from an array of strings.

## Usage

``` r
librdf_new_hash_from_array_of_strings ( world,
  name,
  string )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- name:

  hash name ("character")

- string:

  address of the start of the array of char\* pointers ("character")

## Value

\_p_librdf_hash_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
