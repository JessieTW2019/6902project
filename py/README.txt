# comp6902proj


## Directory layout

* CNFVarManager: Keeps track of the meaning of the cnf variables  
* get_clause_count: analytically compute # of clauses which will be produced for given parameter settings  
* graph_generator: used to generate random graphs  
* graph_tools: useful graph functions for other files (loading, printing, ect)  
* reduce_to_clique: creates an instance of the k-clique problem from an instance of k common subgraph. outputs clique instance to ../cliques directory  
* reduce_to_sat: creates an instance of the cnf sat problem from an instance of k common subgraph. outputs the cnf sat instance to ../cnf directory  


## Running Scripts (See individual files for more info on parameters)

* graph_generator: python3 graph_generator.py <mo> <m> <n> <alpha> <graph_id>
outputs graph to ../graphs/graph_id

* reduce_to_clique: python3 reduce_to_clique.py <graph_g_id> <graph_h_id> <k> <out_id>
graph_g_id, graph_h_id are names of files containing graphs in ../graphs
outputs clique_instance to ../cliques

* reduce_to_sat: <graph_g_id> <graph_h_id> <k> <out_id>
graph_g_id, graph_h_id are names of files containing graphs in ../graphs
outputs clique_instance to ../cliques