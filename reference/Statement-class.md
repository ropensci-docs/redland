# An RDF Statement object

A Statement object is created using the provided subject, predicate and
object.

## Details

A Statement object can be created from Node objects that are provided
for the subject, predicate and object. An alternative way to create a
Statement object is to provide the subject, predicate and object as
character values. If this later method is used, the character values
will be evaluated to determine the appropriate RDF type for the subject
and object. Note that the RDF type for the predicate will always be
'uri' (aka 'resource'). If the automatic determination of RDF types is
not desired, then the `subjectType` and `objectType` parameters can be
specified to explicitly set the RDF types.

## Slots

- `librdf_statement`:

  A redland statement object

## Methods

- [`Statement-initialize`](https://docs.ropensci.org/redland/reference/Statement-initialize.md):
  Initialize a Statement object.
  [`getTermType`](https://docs.ropensci.org/redland/reference/getTermType.md):
  Return the redland node type for the specified RDF term in a
  statement.
  [`freeStatement`](https://docs.ropensci.org/redland/reference/freeStatement.md):
  Free memory used by a librdf statement.

## See also

[`redland`](https://docs.ropensci.org/redland/reference/redland.md):
redland package

## Examples

``` r
world <- new("World")
# Create nodes manually and add to the statment
subject <- new("Node", blank="_:myid1", world)
predicate <- new("Node", uri="http://www.example.com/isa", world)
object <- new("Node", literal="thing", world)
stmt <- new("Statement", world, subject, predicate, object)

# Create the statement specifying node values directly
stmt <- new("Statement", world, subject="http://www.example.com/myevent",
                                predicate="http://example.com/occurredAt",
                                object="Tue Feb 17 14:05:13 PST 2015")
stmt <- new("Statement", world, subject=NULL, 
                                predicate="http://www.example.com/hasAddr",
                                object="http://www.nothing.com", objectType="literal")
stmt <- new("Statement", world, subject="http://www.example.com/BobSmith", 
                                predicate="http://www.example.com/says",
                                object="¡Hola, amigo! ¿Cómo estás?", 
                                objectType="literal",
                                language="es")
```
