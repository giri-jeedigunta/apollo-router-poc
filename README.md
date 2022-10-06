# Federation with Apollo Router 

A super simple GraphQL federation with Apollo Router. Reusing dummy subgraphs for this example from the official docs / examples: - [apollographql/supergraph-demo](https://github.com/apollographql/supergraph-demo). 

## Local setup(macOS): 
### Prerequisite(macOS):     
 - Install rover: `curl -sSL https://rover.apollo.dev/nix/latest | sh`

 ### Run locally:     
 - Install router in the root folder `curl -sSL https://router.apollo.dev/download/nix/latest | sh`
 - Optinal: To generate subgraph run `rover --log trace supergraph compose --config supergraph.yaml > supergraph.graphql`
 - Start all the subgraphs servers in the subgraphs folder. 
 - Run the apollo router using `./router --dev --hr --supergraph supergraph.graphql`
 - Open `http://localhost:4000/` you can interactively query your subgraphs.
