# Load content from a URI into the model.

Load content from a URI into the model.

## Usage

``` r
librdf_model_load ( model,
  uri,
  name,
  mime_type,
  type_uri,
  .copy )
```

## Arguments

- model:

  librdf_model object ("\_p_librdf_model_s")

- uri:

  the URI to read the content ("\_p_librdf_uri_s")

- name:

  the name of the parser (or NULL) ("character")

- mime_type:

  the MIME type of the syntax (NULL if not used) ("character")

- type_uri:

  URI identifying the syntax (NULL if not used) ("\_p_librdf_uri_s")

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
