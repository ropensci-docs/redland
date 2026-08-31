# A Redland World object, used to initialize the Redland RDF library.

A World object is the top level object in the Redland RDF library
implementation, so it contains all other objects needed to process RDF
Models.

## Slots

- `librdf_world`:

  A redland world object

## Methods

- [`World-initialize`](https://docs.ropensci.org/redland/reference/World-initialize.md):
  Initialize a World object
  [`freeWorld`](https://docs.ropensci.org/redland/reference/freeWorld.md):
  Free memory used by a librdf world object

## See also

[`redland`](https://docs.ropensci.org/redland/reference/redland.md):
redland package

## Examples

``` r
world <- new("World")
```
