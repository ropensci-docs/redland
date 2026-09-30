# Constructor - create a new storage librdf_model object.

Constructor - create a new storage librdf_model object.

## Usage

``` r
librdf_new_model ( world,
  storage,
  options_string )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- storage:

  librdf_storage to use ("\_p_librdf_storage_s")

- options_string:

  options to initialise model ("character")

## Value

\_p_librdf_model_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
