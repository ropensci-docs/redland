# Create and add a new statement about a resource to the model.

Create and add a new statement about a resource to the model.

## Usage

``` r
librdf_model_add ( model,
  subject,
  predicate,
  object,
  .copy )
```

## Arguments

- model:

  model object ("\_p_librdf_model_s")

- subject:

  librdf_node of subject ("\_p_librdf_node_s")

- predicate:

  librdf_node of predicate ("\_p_librdf_node_s")

- object:

  librdf_node of object (literal or resource) ("\_p_librdf_node_s")

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
