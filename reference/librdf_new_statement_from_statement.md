# Copy constructor - create a new librdf_statement from an existing librdf_statement. Creates a deep copy - changes to original statement nodes are not reflected in the copy.

Copy constructor - create a new librdf_statement from an existing
librdf_statement. Creates a deep copy - changes to original statement
nodes are not reflected in the copy.

## Usage

``` r
librdf_new_statement_from_statement ( statement )
```

## Arguments

- statement:

  librdf_statement to copy ("\_p_librdf_statement_s")

## Value

\_p_librdf_statement_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
