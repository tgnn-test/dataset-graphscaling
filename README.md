# dataset-graphscaling

Interactive version [here](https://tgnn-test.github.io/)

## Structure
`graph-generation`:
* generated graphs
* divided by method:
  * Netgan
  * BiGG
  * GraphRNN
  * GSM
  * GraphGDP

`graph-upscaling`:
* up-scaled graphs
* divided by method and scale:
  * Kronecker:
    * scales 2-256
  * Gscaler:
    * scales 2-256
  * EvoGraph:
    * scales 2-256

## Use the Data

All graphs are stored as a pickled list of networkx graphs.

You can load graphs using the following code:

```python
import pickle
import networkx as nx

with open(filename, 'rb') as f:
    graphs = pickle.load(f)
    print(type(graphs[0]))
```

```bash
<class 'networkx.classes.graph.Graph'>
```

## Cite

```bash
@inproceedings{Helm2310:Synthesizing,
  author = {Helm, Max and Carle, Georg},
  title = {{Synthesizing and Scaling WAN Topologies using Permutation-invariant Graph Generative Models}},
  booktitle = {19th International Conference on Network and Service Management (CNSM 2023)},
  address = {Niagara Falls, Canada},
  pages = 6,
  days = 30,
  month = oct,
  year = 2023,
  month_numeric = 10
}
```
