# Parse a string of content into an librdf_model.

Parse a string of content into an librdf_model.

## Usage

``` r
librdf_parser_parse_string_into_model ( parser,
  string,
  base_uri,
  model,
  .copy )
```

## Arguments

- parser:

  the parser ("\_p_librdf_parser_s")

- string:

  the content to parse ("character")

- base_uri:

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
