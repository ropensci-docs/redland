# Set the world log handling function.

Set the world log handling function.

## Usage

``` r
librdf_world_set_logger ( world,
  user_data,
  log_handler )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- user_data:

  user data to pass to function ("\_p_void")

- log_handler:

  pointer to the function ("\_p_librdf_log_func")

## Value

void

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
