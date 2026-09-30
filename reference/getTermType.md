# Return the redland node type for the specified RDF term in a statement

After a Statement object has been created, this method can be used to
determine the RDF type ("uri", "literal", "blank") that has been
assigned to the specified RDF term, i.e. "subject", "predicate",
"object".

## Usage

``` r
getTermType(.Object, term)

# S4 method for class 'Statement,character'
getTermType(.Object, term)
```

## Arguments

- .Object:

  a Statement object

- term:

  the RDF term for which the type will be returned

## Examples

``` r
world <- new("World")
subject <- new("Node", blank="_:myid1", world)
predicate <- new("Node", uri="http://www.example.com/isa", world)
object <- new("Node", literal="thing", world)
stmt <- new("Statement", world, subject, predicate, object, world)
termType <- getTermType(stmt, "predicate")
```
