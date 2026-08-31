# Create and add a new statement about a literal to the model.

Create and add a new statement about a literal to the model.

## Usage

``` r
librdf_model_add_string_literal_statement ( model,
  subject,
  predicate,
  literal,
  inStrOrNull,
  is_wf_xml,
  .copy )
```

## Arguments

- model:

  model object ("\_p_librdf_model_s")

- subject:

  librdf_node of subject ("\_p_librdf_node_s")

- predicate:

  librdf_node of predicate ("\_p_librdf_node_s")

- literal:

  string literal conten ("character")

- inStrOrNull:

  language of literal ("character")

- is_wf_xml:

  literal is XML ("integer")

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
