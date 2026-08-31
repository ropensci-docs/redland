# Free memory used by a librdf world object

Free memory used by a librdf world object

## Usage

``` r
freeWorld(.Object)

# S4 method for class 'World'
freeWorld(.Object)
```

## Arguments

- .Object:

  a World object

## Details

After this method is called, the World object is no longer usable and
should be deleted `"rm(world)"` and a new object created.

## Examples

``` r
world <- new("World")
# At this point we would perform some operations using the world object.
# When the world object is no longer needed, we can free the resources it has allocated.
result <- freeWorld(world)
rm(world)
```
