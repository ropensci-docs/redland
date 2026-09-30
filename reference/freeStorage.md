# Free memory used by a librdf storage object

After this method is called, the Storage object is no longer usable and
should be deleted `"rm(storage)"` and a new object created.

## Usage

``` r
freeStorage(.Object)

# S4 method for class 'Storage'
freeStorage(.Object)
```

## Arguments

- .Object:

  a Storage object to free memory for

## Examples

``` r
world <- new("World")
storage <- new("Storage", world, "hashes", name="", options="hash-type='memory'")
# At this point we would perform some operations using the storage object.
# See '?redland' for a complete example.
# When the Storage object is no longer needed, the resources it had allocated can be freed.
status <- freeStorage(storage)
rm(storage)
```
