# Set the value of a parser feature.

Set the value of a parser feature.

## Usage

``` r
librdf_parser_set_feature ( parser,
  feature,
  value,
  .copy )
```

## Arguments

- parser:

  librdf_parser object ("\_p_librdf_parser_s")

- feature:

  librdf_uri feature property ("\_p_librdf_uri_s")

- value:

  librdf_node feature property value ("\_p_librdf_node_s")

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
