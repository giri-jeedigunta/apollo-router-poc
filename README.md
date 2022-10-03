# Federation with Apollo Router 

A super simple GraphQL federation with Apollo Router. Subgraphs for this example are borrowed from the official repo: - [apollographql/supergraph-demo](https://github.com/apollographql/supergraph-demo). 

## Prerequisite: 

Install rover: `curl -sSL https://rover.apollo.dev/nix/latest | sh`


## Local setup: 

- To generate subgraph run `rover --log trace supergraph compose --config supergraph.yaml > supergraph.graphql`
- Start all the subgraphs servers in the subgraphs folder. Once everytning is up and running, run the apollo router using `./router --dev --supergraph supergraph.graphql`
 - open `http://localhost:4000/` you can interactively query your subgraphs.
