# Initialize a Storage object

Initialize a Storage object

## Usage

``` r
# S4 method for class 'Storage'
initialize(
  .Object,
  world,
  type = "hashes",
  name = "",
  options = "hash-type='memory'"
)
```

## Arguments

- .Object:

  the Storage object

- world:

  the World object

- type:

  the Redland storage type

- name:

  storage instance name

- options:

  storage options

## Value

the Storage object

## Examples

``` r
world <- new("World")
storage <- new("Storage", world, "hashes", name="", options="hash-type='memory'")
```
