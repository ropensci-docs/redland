# Parse a counted string of content to a librdf_stream of statements.

Parse a counted string of content to a librdf_stream of statements.

## Usage

``` r
librdf_parser_parse_counted_string_as_stream ( parser,
  string,
  length,
  base_uri )
```

## Arguments

- parser:

  the parser ("\_p_librdf_parser_s")

- string:

  the string to parse ("character")

- length:

  length of the string content (must be \>0) ("integer")

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
