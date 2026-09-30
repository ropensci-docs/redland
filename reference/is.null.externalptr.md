# Determine whether an externalptr object is NULL.

The pointer is treated as an externalptr and checked via a call in C to
see if it is NULL.

## Usage

``` r
is.null.externalptr(pointer)
```

## Arguments

- pointer:

  externalptr to be checked for NULL value

## Value

logical TRUE if the pointer is NULL, otherwise FALSE
