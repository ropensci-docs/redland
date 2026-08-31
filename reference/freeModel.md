# Free memory used by a librdf model.

Free memory used by a librdf model.

## Usage

``` r
freeModel(.Object)

# S4 method for class 'Model'
freeModel(.Object)
```

## Arguments

- .Object:

  a Model object

## Details

After this method is called, the Model object is no longer usable and
should be deleted `"rm(model)"` and a new object created.

## Examples

``` r
world <- new("World")
storage <- new("Storage", world, "hashes", name="", options="hash-type='memory'")
model <- new("Model", world, storage, options="")
# At this point, some operations would be performed with the model.
# See '?redland' for a complete example.
# When the Model object is no longer needed, the resources it has allocated can be freed.
freeModel(model)
#> NULL
rm(model)
```
