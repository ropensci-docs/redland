# Write a librdf_stream to a file.

Write a librdf_stream to a file.

## Usage

``` r
librdf_serializer_serialize_stream_to_file ( serializer,
  name,
  base_uri,
  stream,
  .copy )
```

## Arguments

- serializer:

  the serializer ("\_p_librdf_serializer_s")

- name:

  filename to serialize to ("character")

- base_uri:

  the base URI to use (or NULL) ("\_p_librdf_uri_s")

- stream:

  the librdf_stream stream to use ("\_p_librdf_stream_s")

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
