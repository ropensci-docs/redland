# Constructor - Create a new librdf_model with storage.

Constructor - Create a new librdf_model with storage.

## Usage

``` r
librdf_new_model_with_options ( world,
  storage,
  options )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- storage:

  librdf_storage storage to use ("\_p_librdf_storage_s")

- options:

  librdf_hash of options to use ("\_p_librdf_hash_s")

## Value

\_p_librdf_model_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
