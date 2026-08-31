# A Redland Storage object

A Redland Storage object

## Slots

- `librdf_storage`:

  A redland storage object

- `type`:

  the storage type to create, i.e. "hashes", "mysql", "postgresql", ...

## Methods

- [`Storage-initialize`](https://docs.ropensci.org/redland/reference/Storage-initialize.md):
  Initialize a Storage object
  [`freeStorage`](https://docs.ropensci.org/redland/reference/freeStorage.md):
  Free memory used by a librdf storage object

## See also

[`redland`](https://docs.ropensci.org/redland/reference/redland.md):
redland package

## Examples

``` r
world <- new("World")
storage <- new("Storage", world, "hashes", name="", options="hash-type='memory'")
```
