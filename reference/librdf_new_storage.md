# Constructor - create a new librdf_storage object.

Constructor - create a new librdf_storage object.

## Usage

``` r
librdf_new_storage ( world,
  storage_name,
  name,
  options_string )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- storage_name:

  the storage factory name ("character")

- name:

  an identifier for the storage ("character")

- options_string:

  options to initialise storage ("character")

## Value

\_p_librdf_storage_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
