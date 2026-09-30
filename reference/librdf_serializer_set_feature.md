# Set the value of a serializer feature.

Set the value of a serializer feature.

## Usage

``` r
librdf_serializer_set_feature ( serializer,
  feature,
  value,
  .copy )
```

## Arguments

- serializer:

  serializer object ("\_p_librdf_serializer_s")

- feature:

  URI of feature ("\_p_librdf_uri_s")

- value:

  value to set ("\_p_librdf_node_s")

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
