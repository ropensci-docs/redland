# Free memory used by a librdf parser

Free memory used by a librdf parser

## Usage

``` r
freeParser(.Object)

# S4 method for class 'Parser'
freeParser(.Object)
```

## Arguments

- .Object:

  a Node object

## Details

After freeNode is called, the Node object is no longer usable and should
be deleted `"rm(nodeName)"` and a new object created.

## Examples

``` r
world <- new("World")
storage <- new("Storage", world, "hashes", name="", options="hash-type='memory'")
model <- new("Model", world, storage, options="")
parser <- new("Parser", world)
filePath <- system.file("extdata/example.rdf", package="redland")
parseFileIntoModel(parser, world, filePath, model)
# At this point, some operations would be performed with the Model that has been populated
# with the parser.
# See '?redland' for a complete example.
# When the parser object is no longer needed, the resources it had allocated can be freed.
freeParser(parser)
#> NULL
rm(parser)
```
