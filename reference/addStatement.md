# Add a Statement object to the Model

Add a Statement object to the Model

## Usage

``` r
addStatement(.Object, statement)

# S4 method for class 'Model,Statement'
addStatement(.Object, statement)
```

## Arguments

- .Object:

  a Model object

- statement:

  the Statement that will be added

## Examples

``` r
world <- new("World")
storage <- new("Storage", world, "hashes", name="", options="hash-type='memory'")
model <- new("Model", world, storage, options="")
```
