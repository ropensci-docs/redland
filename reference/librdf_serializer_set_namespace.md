# Set a namespace URI/prefix mapping.

Set a namespace URI/prefix mapping.

## Usage

``` r
librdf_serializer_set_namespace ( serializer,
  nspace,
  prefix,
  .copy )
```

## Arguments

- serializer:

  serializer object ("\_p_librdf_serializer_s")

- nspace:

  URI of namespace or NULL ("\_p_librdf_uri_s")

- prefix:

  prefix to use or NULL ("character")

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
