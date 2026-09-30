# Constructor - create a new literal librdf_node object.

Constructor - create a new literal librdf_node object.

## Usage

``` r
librdf_new_node_from_literal ( world,
  string,
  inStrOrNull,
  is_wf_xml )
```

## Arguments

- world:

  redland world object ("\_p_librdf_world_s")

- string:

  literal UTF-8 encoded string value ("character")

- inStrOrNull:

  literal XML language (or NULL, empty string) ("character")

- is_wf_xml:

  non 0 if literal is XML ("integer")

## Value

\_p_librdf_node_s

## References

<https://librdf.org/docs/>

## See also

This R function is a wrapper function that directly calls the the
Redland RDF C libraries. For more information about Redland RDF, view
the online documentation indicated in the 'References' section.
