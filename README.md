```python
from collections import Counter
def std(arr):        
    arr = ''.join(sorted([x.lower() if not x.isspace() else '' for x in set(arr)]))
    return arr

def find_uniq(arr):
    org = arr.copy()
    arr = list(map(std, arr))
    index = arr.index( Counter(arr).most_common()[-1][0] )    
    return org[index]
```

- Me gustan los abrazos
- Me gusta Python
- No afiliado a McDonalds
