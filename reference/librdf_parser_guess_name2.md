# Get a parser name for content with type or identifier

Get a parser name for content with type or identifier

## Usage

``` r
librdf_parser_guess_name2 ( world,
  mime_type,
  buffer,
  identifier )
```

## Arguments

- world:

  librdf_world object ("\_p_librdf_world_s")

- mime_type:

  MIME type of syntax or NULL ("character")

- buffer:

  content buffer or NULL ("character")

- identifier:

  content identifier or NULL ("character")

## Value

character

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
