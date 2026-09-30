# Add more data to the librdf_digest object.

Add more data to the librdf_digest object.

## Usage

``` r
librdf_digest_update ( digest,
  buf,
  length )
```

## Arguments

- digest:

  the digest ("\_p_librdf_digest_s")

- buf:

  the data buffer ("character")

- length:

  the length of the data ("integer")

## Value

void

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
