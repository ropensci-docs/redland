# Free memory used by a librdf serializer.

Free memory used by a librdf serializer.

## Usage

``` r
freeSerializer(.Object)

# S4 method for class 'Serializer'
freeSerializer(.Object)
```

## Arguments

- .Object:

  a Serializer object

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
# At this point, some operations would be performed with the Serializer object. 
# See '?Serializer' for a complete example.
# When the serializer object is no longer needed, the resources it had allocated can be freed.
freeSerializer(serializer)
#> NULL
rm(serializer)
```
