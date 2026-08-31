# Compare two librdf_uri objects lexicographically.

Compare two librdf_uri objects lexicographically.

## Usage

``` r
librdf_uri_compare ( first_uri,
  second_uri,
  .copy )
```

## Arguments

- first_uri:

  librdf_uri object 1 or NULL ("\_p_librdf_uri_s")

- second_uri:

  librdf_uri object 2 or NULL ("\_p_librdf_uri_s")

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
