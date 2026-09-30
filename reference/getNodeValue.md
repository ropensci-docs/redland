# Get the value of the node as a string

Get the value of the node as a string

## Usage

``` r
getNodeValue(.Object)

# S4 method for class 'Node'
getNodeValue(.Object)
```

## Arguments

- .Object:

  a Node object

## Value

a string representation of the Node's value

## Details

The value of the node is returned as a string. If the node type is
'blank', then the blank node identifier is returned. If the node type is
'literal', then the literal value is returned with the form
"string@language, e.g. "¡Hola, amigo! ¿Cómo estás?"@es". If the node
type is 'uri' then the value is returned as a string.

## Examples

``` r
world <- new("World")
node <- new("Node", world, literal="¡Hola, amigo! ¿Cómo estás?", language="es")
value <- getNodeValue(node)
```
