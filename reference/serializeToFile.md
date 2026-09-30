# Serialize a model to a file.

Serialize a model to a file.

## Usage

``` r
serializeToFile(.Object, world, model, filePath, ...)

# S4 method for class 'Serializer,World,Model,character'
serializeToFile(.Object, world, model, filePath, baseUri = as.character(NA))
```

## Arguments

- .Object:

  a Serializer object

- world:

  a World object

- model:

  a Model object

- filePath:

  a file path that the serialized model will be written to

- ...:

  Additional parameters

- baseUri:

  a base URI to use for the serialization

## Value

an integer containing the return status where non zero indicates an
error occurred during serialization
