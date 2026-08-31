# Write a serialized librdf_model to a string. The returned string must be freed by the caller using librdf_free_memory().

Write a serialized librdf_model to a string. The returned string must be
freed by the caller using librdf_free_memory().

## Usage

``` r
librdf_serializer_serialize_model_to_string ( serializer,
  inUriOrNull,
  model )
```

## Arguments

- serializer:

  the serializer ("\_p_librdf_serializer_s")

- inUriOrNull:

  the base URI to use (or NULL) ("\_p_librdf_uri_s")

- model:

  the librdf_model model to use ("\_p_librdf_model_s")

## Value

character

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
