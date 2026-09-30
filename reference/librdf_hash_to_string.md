# Format the hash as a string, suitable for parsing by librdf_hash_from_string.

Format the hash as a string, suitable for parsing by
librdf_hash_from_string.

## Usage

``` r
librdf_hash_to_string ( hash,
  filter )
```

## Arguments

- hash:

  librdf_hash object ("\_p_librdf_hash_s")

- filter:

  NULL terminated list of keys to ignore ("\_p_p_char")

## Value

character

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
