# Initialize a Node object.

A Node has an associated type corresponding to the RDF component that it
is representing. The list of possible types is "resource", "literal" or
"blank".

## Usage

``` r
# S4 method for class 'Node'
initialize(.Object, world, literal, uri, blank, datatype_uri, language)
```

## Arguments

- .Object:

  the Node object to be initialized

- world:

  a World object

- literal:

  a literal character value to be assigned to the node

- uri:

  a uri character value to be assigned to the node

- blank:

  a blank node identifier to be assigned to the node

- datatype_uri:

  a uri used to specify the datatype of a literal node, i.e.
  "http://www.w3.org/2001/XMLSchema#string"

- language:

  a character value specifying the RDF language tag (excluding the "@"
  symbol), i.e. "fr"

## Value

the Node object

## Details

The url=' and 'literal=' arguments determine which type of Node is
created. The Node type affects how the Node is processed in
serialization, for example a Node created with 'node1 \<- new("Node",
literal="http://www.example.com")' is processed differently that a Node
created with 'node1 \<- new("Node", url="http://www.example.com")', with
the former being processed as an RDF literal and the latter processed as
an RDF resource.

## Note

Refer to https://www.w3.org/TR/rdf11-concepts information on language
tags.
