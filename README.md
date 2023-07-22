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
