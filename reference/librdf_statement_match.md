# Match a statement against a 'partial' statement.

Match a statement against a 'partial' statement.

## Usage

``` r
librdf_statement_match ( statement,
  partial_statement,
  .copy )
```

## Arguments

- statement:

  statement ("\_p_librdf_statement_s")

- partial_statement:

  statement with possible empty parts ("\_p_librdf_statement_s")

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
