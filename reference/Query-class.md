# Query an RDF model

The Query class is used to execute a query on a Model object using the
default query language SPARQL. For more information, please refer to
<https://librdf.org/rasqal/> for details on supported query languages.

## Details

A Query is executed using the executeQuery method, which returns a
QueryResults object that can be iterated over the query solution
sequence.

## Slots

- `librdf_query`:

  A redland query object

- `librdf_world`:

  A redland world object

## Methods

- [`Query-initialize`](https://docs.ropensci.org/redland/reference/Query-initialize.md):
  Initialize a Query object.
  [`executeQuery`](https://docs.ropensci.org/redland/reference/executeQuery.md):
  Execute a query.
  [`setQueryResultLimit`](https://docs.ropensci.org/redland/reference/setQueryResultsLimit.md):
  Set limit on returned query results.
  [`getQueryResultLimit`](https://docs.ropensci.org/redland/reference/getQueryResultsLimit.md):
  Get the query result limit.
  [`getResults`](https://docs.ropensci.org/redland/reference/getResults.md):
  Return all query results.
  [`writeResults`](https://docs.ropensci.org/redland/reference/writeResults.md):
  Write query results to a file.
  [`freeParser`](https://docs.ropensci.org/redland/reference/freeParser.md):
  Free memory used by a librdf query.

## References

www.example.com

## See also

[`redland`](https://docs.ropensci.org/redland/reference/redland.md):
redland package

## Examples

``` r
world <- new("World")
storage <- new("Storage", world, "hashes", name="", options="hash-type='memory'")
model <- new("Model", world, storage, options="")
stmt <- new("Statement", world=world, 
  subject="https://cn.dataone.org/cn/v1/resolve/urn:uuid:274a0c5c-3082-4562-bbd3-2b1288768cac",
  predicate="http://www.w3.org/ns/prov#hadPlan",
  object="https://cn.dataone.org/cn/v1/resolve/urn:uuid:01305f45-f22b-40c8-8d27-00357d01e4a5")
status <- addStatement(model, stmt)
stmt <- new("Statement", world=world, 
           subject="https://orcid.org/0000-0002-2192-403X",
           predicate="http://www.w3.org/ns/prov#Agent",
           object="slaughter", 
           objectType="literal", 
           datatype_uri="http://www.w3.org/2001/XMLSchema#string")
status <- addStatement(model, stmt)
queryString <- 
    paste("PREFIX orcid: <https://orcid.org/>",
          "PREFIX dataone: <https://cn.dataone.org/cn/v1/resolve/>",
          "PREFIX prov: <http://www.w3.org/ns/prov#>",
          "SELECT ?a ?c WHERE { ?a prov:Agent ?c . }", sep=" ")
query <- new("Query", world, queryString, base_uri=NULL, query_language="sparql", query_uri=NULL)
# Return all results as a string
results <- getResults(query, model, "rdfxml")
```
