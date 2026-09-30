# Determine the node type and return as a string

A Node has a type that is assigned at initialization and can have one of
the following values: 'resource', 'literal', 'blank' and 'unknown'.

## Usage

``` r
getNodeType(.Object)

# S4 method for class 'Node'
getNodeType(.Object)
```

## Arguments

- .Object:

  a Node object

## Value

a character vector containing the Node type

## Examples

``` r
world <- new("World")
node <- new("Node", world, uri="http://www.example.com")
nodeType <- getNodeType(node)
```
