# Constructor - create a new librdf_serializer object.

Constructor - create a new librdf_serializer object.

## Usage

``` r
librdf_new_serializer ( world,
  name,
  mime_type,
  type_uri )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- name:

  the serializer factory name (or NULL or empty string if don't care)
  ("character")

- mime_type:

  the MIME type of the syntax (NULL if not used) ("character")

- type_uri:

  URI of syntax (NULL if not used) ("\_p_librdf_uri_s")

## Value

\_p_librdf_serializer_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
