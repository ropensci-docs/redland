# An RDF Parser object

The Parser class provides methods to parse RDF content into a Redland
RDF model.

## Slots

- `librdf_parser`:

  A redland parser object

## Methods

- [`Parser-initialize`](https://docs.ropensci.org/redland/reference/Parser-initialize.md):
  Initialize a Parser object.
  [`parseFileIntoModel`](https://docs.ropensci.org/redland/reference/parseFileIntoModel.md):
  Parse the contents of a file into a model.
  [`freeParser`](https://docs.ropensci.org/redland/reference/freeParser.md):
  Free memory used by a librdf parser.

## See also

[`redland`](https://docs.ropensci.org/redland/reference/redland.md):
redland package

## Examples

``` r
world <- new("World")
storage <- new("Storage", world, "hashes", name="", options="hash-type='memory'")
model <- new("Model", world, storage, options="")
# Create the default "rdfxml" parser
parser <- new("Parser", world)
filePath <- system.file("extdata/example.rdf", package="redland")
parseFileIntoModel(parser, world, filePath, model)
```
