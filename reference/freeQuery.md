# Free memory used by a librdf query

Free memory used by a librdf query

## Usage

``` r
freeQuery(.Object)

# S4 method for class 'Query'
freeQuery(.Object)
```

## Arguments

- .Object:

  a Query object

## Details

After this method is called, the Query object is no longer usable and
should be deleted `"rm(query)"` and a new object created.

## Examples

``` r
world <- new("World")
storage <- new("Storage", world, "hashes", name="", options="hash-type='memory'")
model <- new("Model", world, storage, options="")
stmt <- new("Statement", world=world, 
  subject="https://orcid.org/0000-0002-2192-403X",
  predicate="http://www.w3.org/ns/prov#Agent",
  object="slaughter", 
  objectType="literal", datatype_uri="http://www.w3.org/2001/XMLSchema#string")
status <- addStatement(model, stmt)
queryString <- paste("PREFIX orcid: <https://orcid.org/>",
                     "PREFIX dataone: <https://cn.dataone.org/cn/v1/resolve/>",
                     "PREFIX prov: <http://www.w3.org/ns/prov#>",
                     "SELECT ?a ?c WHERE { ?a prov:Agent ?c . }", sep=" ")
query <- new("Query", world, queryString, base_uri=NULL, 
  query_language="sparql", query_uri=NULL)
# Return all results as a string
results <- getResults(query, model, "rdfxml")

# When the query object is no longer needed, the resources it had allocated can be freed.
freeQuery(query)
#> NULL
rm(query)
```
