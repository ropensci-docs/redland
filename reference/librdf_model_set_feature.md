# Set the value of a graph feature.

Set the value of a graph feature.

## Usage

``` r
librdf_model_set_feature ( model,
  feature,
  value,
  .copy )
```

## Arguments

- model:

  librdf_model object ("\_p_librdf_model_s")

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
