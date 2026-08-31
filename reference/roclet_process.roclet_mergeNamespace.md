# Roxygen process function for the 'mergeNamespace' roclet

This function is called by the Roxygen2 roxygenize function.

## Usage

``` r
# S3 method for class 'roclet_mergeNamespace'
roclet_process(x, blocks, env, base_path)
```

## Arguments

- x:

  the currently running roclet

- blocks:

  the documentation blocks

- env:

  the current env

- base_path:

  the top directory of the R package

## Details

This function loads the Redland interface file and tests each loaded
function to see if it should be exported via the NAMESPACE file.
