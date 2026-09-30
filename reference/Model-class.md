# A Redland Model object

A Model object is used to store the statements (triples) of an RDF
model.

## Details

A Model may be created manually by creating
[`Statement`](https://docs.ropensci.org/redland/reference/Statement-class.md)
and adding them to the Model using
[`addStatement`](https://docs.ropensci.org/redland/reference/addStatement.md),
or a Model may be read in from a previously saved file using
[`parseFileIntoModel`](https://docs.ropensci.org/redland/reference/parseFileIntoModel.md).
Once a Model is created, it can be queried using
[`Query`](https://docs.ropensci.org/redland/reference/Query-class.md).

## Slots

- `librdf_model`:

  A redland model object

## Methods

- [`Model-initialize`](https://docs.ropensci.org/redland/reference/Model-initialize.md):
  Initialize a Model object
  [`addStatement`](https://docs.ropensci.org/redland/reference/addStatement.md):
  Add a Statement object to the Model
  [`freeModel`](https://docs.ropensci.org/redland/reference/freeModel.md):
  Free memory used by a librdf model object

## See also

View examples of creating models by viewing the `'redland_overview'`
vignette: `'vignette("redland_overview")'`

[`redland`](https://docs.ropensci.org/redland/reference/redland.md):
redland package

## Examples

``` r
world <- new("World")
storage <- new("Storage", world, "hashes", name="", options="hash-type='memory'")
model <- new("Model", world, storage, options="")
```
