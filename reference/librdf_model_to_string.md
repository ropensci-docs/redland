# Write serialized model to a string.

Write serialized model to a string.

## Usage

``` r
librdf_model_to_string ( model,
  uri,
  name,
  mime_type,
  inUriOrNull )
```

## Arguments

- model:

  librdf_model object ("\_p_librdf_model_s")

- uri:

  base URI to use in serializing (or NULL if not used)
  ("\_p_librdf_uri_s")

- name:

  the name of the serializer (or NULL for default) ("character")

- mime_type:

  the MIME type of the syntax (NULL if not used) ("character")

- inUriOrNull:

  URI identifying the syntax (NULL if not used) ("\_p_librdf_uri_s")

## Value

character

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
