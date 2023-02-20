## Compile the code

```sh
$ make clean
$ make
```
It generates an executable "ged".

## Run the code

You can find how to use the code by
```sh
$ ./ged -h
```

An example of graph similarity search on the AIDS dataset with threshold 5 is as follows
```sh
$ ./ged -d datasets/AIDS.txt -q datasets/AIDS_query100.txt -m search -p astar -l LSa -t 5
``` 

## Data format
t [starts a new graph, followed by two arbitrary strings]

v [vertex_id] [vertex_label]

e [vertex_id1] [vertex_id2] [edge_label]

[graph_q.txt](datasets/graph_q.txt) and [graph_g.txt](datasets/graph_g.txt) are two example data files. Note that, vertex_id must be consecutive numbers starting from 0.
