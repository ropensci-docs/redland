# redland: create, query and write RDF graphs

## Introduction

The `redland` R package provides methods to create, query and write to
disk data stored in the Resource Description Framework (RDF). RDF
provides a standardized way to make statements about resources and the
relationships between them. Typical resources include datasets that are
available via URLs. Resources don’t have to be available online, for
example a resource could also be the name of the person that created a
dataset. A collection of RDF statements comprise an RDF graph, which can
be read and interpreted by an RDF capable software application that uses
the resources described in the graph.

An introduction to RDF can be found at
<https://www.w3.org/TR/2014/NOTE-rdf11-primer-20140624/>.

## Examples

The following example reads an RDF graph from a disk file that was
previously saved in the RDF/XML format:

``` r

library(redland)
world <- new("World")
storage <- new("Storage", world, "hashes", name="", options="hash-type='memory'")
model <- new("Model", world=world, storage, options="")
parser <- new("Parser", world)
parseFileIntoModel(parser, world, system.file("extdata", "dc.rdf", package="redland"), model)
```

Next the RDF graph is queried for statements of interest, using the
[SPARQL query syntax](https://www.w3.org/TR/rdf-sparql-query/)

``` r

queryString <- 'PREFIX dc: <http://purl.org/dc/elements/1.1/> SELECT ?a ?c WHERE { ?a dc:creator ?c . }'
query <- new("Query", world, queryString, base_uri=NULL, query_language="sparql", query_uri=NULL)
queryResult <- executeQuery(query, model)
results <- getResults(query, model, "rdfxml")

cat(sprintf("Results from query: %s\n", results))
```

    ## Results from query: <?xml version="1.0" encoding="utf-8"?>
    ## <rdf:RDF xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
    ##    xmlns:rs="http://www.w3.org/2001/sw/DataAccess/tests/result-set#">
    ##   <rs:ResultSet>
    ##     <rs:resultVariable>a</rs:resultVariable>
    ##     <rs:resultVariable>c</rs:resultVariable>
    ##     <rs:solution>
    ##       <rdf:Description>
    ##         <rs:binding>
    ##           <rdf:Description>
    ##             <rs:value rdf:resource="http://www.dajobe.org/"/>
    ##             <rs:variable>a</rs:variable>
    ##           </rdf:Description>
    ##         </rs:binding>
    ##         <rs:binding>
    ##           <rdf:Description>
    ##             <rs:value>Dave Beckett</rs:value>
    ##             <rs:variable>c</rs:variable>
    ##           </rdf:Description>
    ##         </rs:binding>
    ##       </rdf:Description>
    ##     </rs:solution>
    ##   </rs:ResultSet>
    ## </rdf:RDF>

Next, additional statements can be added to the RDF graph:

``` r

stmt <- new("Statement", world=world, 
        subject="http://www.dajobe.org/",
        predicate="http://purl.org/dc/elements/1.1/language",
        object="en")
addStatement(model, stmt)
```

    ## [1] 0

Now the RDF graph can be written to disk:

``` r

serializer <- new("Serializer", world, mimeType="application/rdf+xml")
status <- setNameSpace(serializer, world, namespace="http://purl.org/dc/elements/1.1/", prefix="dc")  
filePath <- tempfile(pattern = "file", tmpdir = tempdir(), fileext = ".rdf")
status <- serializeToFile(serializer, world, model, filePath)
```
