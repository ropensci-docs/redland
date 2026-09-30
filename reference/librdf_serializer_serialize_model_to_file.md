# Write a serialized librdf_model to a file.

Write a serialized librdf_model to a file.

## Usage

``` r
librdf_serializer_serialize_model_to_file ( serializer,
  name,
  inUriOrNull,
  model,
  .copy )
```

## Arguments

- serializer:

  the serializer ("\_p_librdf_serializer_s")

- name:

  filename to serialize to ("character")

- inUriOrNull:

  the base URI to use (or NULL) ("\_p_librdf_uri_s")

- model:

  the librdf_model model to use ("\_p_librdf_model_s")

- .copy:

  NA

## Value

integer

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
