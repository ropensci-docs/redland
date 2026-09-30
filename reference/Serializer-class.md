# An RDF Serializer object.

The Serializer class provides methods to convert a Model object to other
forms, for example, write out a Model to a file.

## Slots

- `librdf_serializer`:

  A redland statement object

## Methods

- [`Serializer-initialize`](https://docs.ropensci.org/redland/reference/Serializer-initialize.md):
  Initialize a Serializer object.
  [`setNameSpace`](https://docs.ropensci.org/redland/reference/setNameSpace.md):
  Set a namespace for the serializer.
  [`serializeToCharacter`](https://docs.ropensci.org/redland/reference/serializeToCharacter.md):
  Serialize a model to a character vector.
  [`serializeToFile`](https://docs.ropensci.org/redland/reference/serializeToFile.md):
  Serialize a model to a file.
  [`freeSerializer`](https://docs.ropensci.org/redland/reference/freeSerializer.md):
  Free memory used by a librdf serializer.

## See also

[`redland`](https://docs.ropensci.org/redland/reference/redland.md):
redland package

## Examples

``` r
world <- new("World")
storage <- new("Storage", world, "hashes", name="", options="hash-type='memory'")
model <- new("Model", world, storage, options="")
filePath <- system.file("extdata/example.rdf", package="redland")
parser <- new("Parser", world)
parseFileIntoModel(parser, world, filePath, model)
# Creat the default "rdfxml" serizlizer
serializer <- new("Serializer", world)
# Add a namespace definition to the serializer
status <- setNameSpace(serializer, world, namespace="http://purl.org/dc/elements/1.1/", prefix="dc")
rdf <- serializeToCharacter(serializer, world, model, baseUri="")
```
