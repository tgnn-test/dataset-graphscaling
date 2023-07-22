# dataset-graphscaling

## Structure
`graph-generation`: TODO

`graph-upscaling`: 

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
