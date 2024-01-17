# Description
Implement multiple compare with python.

# Download
`pip install multiCompare`

# Sample
```
import multiCompare
import pandas as pd

data = {
    "T1": [6.21, 6.13, 5.99, 6.11],
    "T2": [8.25, 8.21, 8.14, 8.34],
    "T3": [7.89, 7.99, 8.10, 7.97],
    "T4": [6.34, 6.52, 6.14, 6.32],
    "T5": [7.89, 7.86, 7.92, 7.80],
    "T6": [7.45, 7.52, 7.47, 7.49],
    "EX": [8.5, 8.5, 8.49, 8.48]
}

df = pd.DataFrame(data)

# Show kruskal result
result = multiCompare.kruskal(df)
print(result)

# Show multiple compare result
score = multiCompare.compare(df, result)
print(score)

```
