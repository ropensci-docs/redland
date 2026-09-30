# Parse the contents of a file into a model

The contents of a the specified file are read and parsed into the
initialized Parser object

## Usage

``` r
parseFileIntoModel(.Object, world, filePath, model, ...)

# S4 method for class 'Parser,World,character,Model'
parseFileIntoModel(.Object, world, filePath, model, baseUri = as.character(NA))
```

## Arguments

- .Object:

  a Parser object

- world:

  a World object

- filePath:

  a file that contains the RDF content

- model:

  a Model object to parse the RDF content into

- ...:

  (Additional parameters)

- baseUri:

  a base URI (i.e. XML base) to apply to the model

## Details

The parser factory name specified during initialization determines how
the content is parsed, for example, if 'rdfxml' was specified during
parser initialization, then the parser expects RDF/XML content as
specified in the W3C recommendation
(http://www.we3.org/TR/REC-rdf-syntax)

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
