# Parse a URI of content into an librdf_model.

Parse a URI of content into an librdf_model.

## Usage

``` r
librdf_parser_parse_into_model ( parser,
  uri,
  inUriOrNull,
  model,
  .copy )
```

## Arguments

- parser:

  the parser ("\_p_librdf_parser_s")

- uri:

  the URI to read the content ("\_p_librdf_uri_s")

- inUriOrNull:

  the base URI to use or NULL ("\_p_librdf_uri_s")

- model:

  the model to use ("\_p_librdf_model_s")

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
