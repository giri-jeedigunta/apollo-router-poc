# Federation with Apollo Router 

A super simple GraphQL federation with Apollo Router. Reusing dummy subgraphs for this example from the official docs / examples: - [apollographql/supergraph-demo](https://github.com/apollographql/supergraph-demo). 

## Prerequisite(macOS): 

Install rover: `curl -sSL https://rover.apollo.dev/nix/latest | sh`

## Local setup(macOS): 
 - Install router `curl -sSL https://router.apollo.dev/download/nix/latest | sh`
 - To generate subgraph run `rover --log trace supergraph compose --config supergraph.yaml > supergraph.graphql`
 - Start all the subgraphs servers in the subgraphs folder. Once everytning is up and running, run the apollo router using `./router --dev --supergraph supergraph.graphql`
 - Open `http://localhost:4000/` you can interactively query your subgraphs.
