# Serialize a model to a character vector.

Serialize a model to a character vector.

## Usage

``` r
serializeToCharacter(.Object, world, model, ...)

# S4 method for class 'Serializer,World,Model'
serializeToCharacter(.Object, world, model, baseUri = as.character(NA))
```

## Arguments

- .Object:

  a Serializer object

- world:

  a World object

- model:

  a Model object

- ...:

  Additional parameters

- baseUri:

  a URI to prepend to relative URIs in the document

## Value

a character vector containing the serialized model
