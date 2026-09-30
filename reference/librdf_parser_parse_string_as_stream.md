# Parse a string of content to a librdf_stream of statements.

Parse a string of content to a librdf_stream of statements.

## Usage

``` r
librdf_parser_parse_string_as_stream ( parser,
  string,
  base_uri )
```

## Arguments

- parser:

  the parser ("\_p_librdf_parser_s")

- string:

  the string to parse ("character")

- base_uri:

  the base URI to use or NULL ("\_p_librdf_uri_s")

## Value

\_p_librdf_stream_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
